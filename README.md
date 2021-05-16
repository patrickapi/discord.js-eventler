# Discord.js'teki Tüm Eventlerin Türkçe Bir Şekilde Anlatımı


Ufak Bilgilendirme :
```js
client.on
```
Kısmını Botunuzu Nasıl Tanımladıysanız Öyle Değiştirceksiniz.



## Mesaj Eventleri (3)


### Message :
Açıklama : Bir Mesaj Atıldığında Çalışır.
```js
client.on("message", message => {
console.log(`${message.content} Adlı Mesaj Atıldı.`)
})
```
### Message Update :
Açıklama : Bir Mesaj Düzenlendiğinde çalışır.
```js
client.on("messageUpdate", (oldMessage,newMessage) => {
console.log(`${oldMessage.content} Adlı Mesaj ${newMessage.content} Olarak Düzenlendi.`)
})
```
### Message Delete :
Açıklama : Bir Mesaj Silindiğinde Çalışır
```js
client.on("messageDelete", (message) => {
console.log(`${message.content} Adlı Mesaj Silindi`)
})
```

## Kanal Eventleri (3)

### Channel Create :
Açıklama : Bir Kanal Oluşturulduğunda Çalışır
```js
client.on("channelCreate", (channel) => {
console.log(`${channel.name} Adlı Kanal Olıştuldu.`)
})
```
### Channel Delete :
Açıklama : Bir Kanal Silindiğinde Çalıır
```js
client.on("channelDelete", (channel) => {
console.log(`${channel.name} Adlı Kanal Silindi.`)
})
```
### Channel Update :
Açıklama : Bir Kanal Güncellendiğinde Çalışır
```js
client.on("channelUpdate", (channel) => {
console.log(`${channel.name} Adlı Kanal Güncellendi.`)
})
```

## Rol Eventleri (3)

### Role Create :
Açıklama : Bir Rol Oluşturulduğunda Çalışır
```js
client.on("roleCreate", (role) => {
console.log(`${role.name} Adlı Kanal Olıştuldu.`)
})
```
### Role Delete :
Açıklama : Bir Rol Silindiğinde Çalıır
```js
client.on("roleDelete", (role) => {
console.log(`${role.name} Adlı Kanal Silindi.`)
})
```
### Role Update :
Açıklama : Bir Rol Güncellendiğinde Çalışır
```js
client.on("roleUpdate", (role) => {
console.log(`${role.name} Adlı Kanal Güncellendi.`)
})
```

## Emoji Eventleri (3)

### Emoji Create :
Açıklama : Bir Emoji Oluşturulduğunda Çalışır
```js
client.on("emojiCreate", (emoji) => {
console.log(`${emoji.name} Adlı Kanal Olıştuldu.`)
})
```
### Emoji Delete :
Açıklama : Bir Emoji Silindiğinde Çalıır
```js
client.on("emojiDelete", (emoji) => {
console.log(`${emoji.name} Adlı Kanal Silindi.`)
})
```
### Emoji Update :
Açıklama : Bir Emoji Güncellendiğinde Çalışır
```js
client.on("emojiUpdate", (emoji) => {
console.log(`${emoji.name} Adlı Kanal Güncellendi.`)
})
```

## Guild Eventleri (8)

### Guild Create :
Açıklama : Bot Bir Sunucuya Katıldığında Çalışır
```js
client.on("guildCreate", (guild) => {
console.log(`${guild.name} Adlı Sunucuya Katıldım.`)
})
```
### Guild Delete :
Açıklama : Bot Bir Sunucudan Atıldığında Çalışır
```js
client.on("guildDelete", (guild) => {
console.log(`${guild.name} Adlı Sunucudan Atıldım.`)
})
```
### Guild Ban Add :
Açıklama : Sunucuda Ban Atıldığında Çalışır.
```js
client.on("guildBanAdd", (guild,user) => {
console.log(`${guild.name} Adlı Sunucuda ${user.username} Adlı Kişi Banlandı.`)
})
```
### Guild Ban Remove :
Açıklama : Sunucuda Ban Kaldırıldığında Çalışır.
```js
client.on("guildBanRemove, (guild,user) => {
console.log(`${guild.name} Adlı Sunucuda ${user.username} Adlı Kişinin Banı Kaldırıldı.`)
})
```
### Guild Update  :
Açıklama : Sunucuda Değişiklik Yapıldığında Çalışır.
```js
client.on("guildBanRemove, (oldGuild,newGuild) => {
console.log(`${oldGuild.name} Düzenlendi.`)
})
```
### Guild Member Add  :
Açıklama : Sunucuya Birisi Katılınca Çalışır.
```js
client.on("guildMemberAdd, (member) => {
console.log(`${member} Sunucuya Katıldı..`)
})
```
### Guild Member Remove  :
Açıklama : Sunucudan Birisi Çıkınca Çalışır.
```js
client.on("guildMemberRemove, (member) => {
console.log(`${member} Sunucudan Ayrıldı.`)
})
```
