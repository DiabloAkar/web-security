# Select nedir?

- Select sizin istediğiniz bir şeyi DB'de aratmanızı sağlar.

### Örnek 1
1. Uç birimi açın
2. `mysql` yazın.
3. `SELECT 1;` yazın fakat enter'a basmayın. Çıkacak olan bilgiyi tahmin etmeye çalışın
- A-) 1 | B-) Syntax Error | C-) Error | D-) SELECT 1 | E-) 0

[Sonuc](https://cdn.discordapp.com/attachments/805191051316297759/895708099669819402/unknown.png)u görmek için tıkla!

### Örnek 2
1. Uç birimi açın
2. `mysql` yazın.
3. `SELECT 2-1;` yazın fakat enter'a basmayın. Çıkacak olan bilgiyi tahmin etmeye çalışın
- A-) 2-1 | B-) Syntax Error | C-) Error | D-) SELECT 1 | E-) 1

[Sonuc](https://cdn.discordapp.com/attachments/805191051316297759/895710257618239498/unknown.png)u görmek için tıkla!

### Örnek 3
1. Uç birimi açın
2. `mysql` yazın.
3. `SELECT '2-1';` yazın fakat enter'a basmayın. Çıkacak olan bilgiyi tahmin etmeye çalışın
- A-) 2-1 | B-) Syntax Error | C-) Error | D-) SELECT 1 | E-) 1

[Sonuc](https://cdn.discordapp.com/attachments/805191051316297759/895715438628073552/unknown.png)u görmek için tıkla!

- Bu şekilde olmasının sebebi " ' ' " içindekileri işleme sokmamasıdır.
### Örnek 4
1. Uç birimi açın
2. `mysql` yazın.
3. `SELECT '2'-'1';` yazın fakat enter'a basmayın. Çıkacak olan bilgiyi tahmin etmeye çalışın
- A-) 2-1 | B-) Syntax Error | C-) Error | D-) SELECT 1 | E-) 1

[Sonuc](https://cdn.discordapp.com/attachments/805191051316297759/895715684271661126/unknown.png)u görmek için tıkla!

- Bu şekilde olma sebebi " ' ' " bir bir ayrıldıkları için ikisini (' ') işleme sokuyor.

### Örnek 5
1. Uç birimi açın
2. `mysql` yazın.
3. `SELECT '2';` yazın fakat enter'a basmayın. Çıkacak olan bilgiyi tahmin etmeye çalışın
- A-) 2-1 | B-) Syntax Error | C-) Error | D-) SELECT 1 | E-) 1

[Sonuc](https://cdn.discordapp.com/attachments/805191051316297759/895715684271661126/unknown.png)u görmek için tıkla!

- Bu şekilde olma sebebi " ' ' " bir bir ayrıldıkları için ikisini (' ') işleme sokuyor.