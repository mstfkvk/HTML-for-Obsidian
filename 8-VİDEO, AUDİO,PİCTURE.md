# video

-> video formatları desteklenmez ise video etiketi arasına ne konulursa onu gösterecektir
-> src: video yolunu gösterir
	poster: video oynatmadan önceki resim
	controls: yazılmazsa kontrol tusları gözükmez
	autoplay: control yazılmazsa sadece 1 kere oynar durur
	loop: sonsuz döngü
	preload: none, kullanıcı basana kadar video yüklenmez
					auto, sayfa yüklendiğinde browser videoyu indirir
					metadata, browser sadece video bigilerini alır
-> source elementi ile birden fazla video veya aynı videonun formatları eklenebilir

```html
<video src="mk.mp4" poster="mk.jpg" preload="auto" controls autoplay width="400" height="400">

    <source src="mk.mp4" type="video/mp4">

    <source src="mk.ogg" type="video/ogg">

    Your browser does not support the video tag.

  </video>
```
![[Pasted image 20220822104053.png]]


# audio

-> herseyiyle yukarının aynısı
```html
<audio controls muted >

    <source src="audio/audio.mp3" type="audio/mpeg" />

    Your browser does not support the audio element.

  </audio>
```
![[Pasted image 20220822105026.png]]

# picture

```html
 <picture>

      <source srcset="images/logo.webp" type="image/webp" />

      <source srcset="images/logo.png" type="image/png" />

      <img src="images/logo.png" alt="logo" />

    </picture>
```


