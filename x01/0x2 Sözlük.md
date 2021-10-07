### SQL Injection Nedir?

Saldırganın web yazılımlarını kullanarak veritabanında kendi istediği veriyi tarama yapmasıdır.

### UNION SQL Injection nedir?

Union komudu ile kendinize özel bir uç birim açmış gibi düşünebilirsiniz.Size tekrardan 'SELECT' birimini kullanmanızı sağlar.

### Error Base SQL Injection nedir?

Örneğin 'http://testphp.vulnweb.com/listproducts.php?cat=1' adresine "...?cat=1" yazan yerin sonuna " ' " koyarsanız
<img src="https://cdn.discordapp.com/attachments/805191051316297759/895691508555079800/unknown.png" width="400" />

hatasını alacaksınız. Bu hata size şunu söylüyor; Database'de taratılan " ' " hatalı olduğunu belirtiliyor. Bu demektir ki bizim yazdığımız her yazı oraya gidiyor. Mantıken biz orada kod çalıştıra biliriz. " ' " Yerine " Diablo " yazdığımda

<img src="https://cdn.discordapp.com/attachments/805191051316297759/895692891010265178/unknown.png" width="400" />

Bize "Diablo"'nun Database'de bir karşılığının olmadığını söylüyor.
Biz buraya bir kaç kod girerek istediğimiz veriyi çekebiliriz.

ÖRNEK"  http://testphp.vulnweb.com/listproducts.php?cat=extractvalue(rand(), concat(1,(SELECT version())))  " yazarsak bize version bilgisini verecektir.

<img src="https://cdn.discordapp.com/attachments/872878976383746059/895689237779869716/unknown.png" width="400" />

Eğer database yazsaydık (" http://testphp.vulnweb.com/listproducts.php?cat=extractvalue(rand(),%20concat(1,(SELECT%20database()))) ")

<img src="https://cdn.discordapp.com/attachments/805191051316297759/895694175805247528/unknown.png" width="400" />

bize database ismini verecektir.
