# Discord.js'teki Tüm Eventlerin Türkçe Bir Şekilde Anlatımı


Ufak Bilgilendirme :
```js
client.on
```
Kısmını Botunuzu Nasıl Tanımladıysanız Öyle Değiştirceksiniz.



## Mesaj Eventleri ()


### Message :
Açıklama : Bir Mesaj Atıldığında Çalışır.
```js
client.on("message", message => {
console.log(`${message.content} Adlı Mesaj Atıldı.`)
})

### Message Update :
Açıklama : Bir Mesaj Düzenlendiğinde çalışır.
```js
client.on("messageUpdate", (oldMessage,newMessage) => {
console.log(`${oldMessage.content} Adlı Mesaj ${newMessage.content} Olarak Düzenlendi.`)
})
