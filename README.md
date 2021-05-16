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

## Kanal Eventleri (4)

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
