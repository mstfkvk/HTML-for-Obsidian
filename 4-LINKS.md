
```html
<a href="http://www.imdb.com">imdb</a>
```

 -> her zaman URL(Uniform Resource Locator) olarak belirtmeye gerek yok
 
```HTML
<a href="index.html">Home</a>
```

### Relative URL's
same folder: (nothing)
child folder:(xxx/xxx)
grandchild folder:(xxx/xxx/xxx)
parent folder:(../xxx)
grandparent folder:(../../xxx) -->> dosyalar bilgisayarda bu sekilde calısır ancak uzak sunucuda çalısmaz.

### Email Link

```html
<a href="mailto:admin@gmail.com" > my personal email </a>
```

###  New Window
- target=" "

```html
<a href="http://imdb.com" target="_blank">imdb</a>

<!--      _blank   -> farklı sekme(tab)'de açar                  -->
<!--      _self    -> default-aynı-tek sekme(tab)'de açar        -->
<!--      _parent  -> başka browser'de açar                      -->
<!--      _top     -> gelişmiş browser'de açar                   -->
```

### id attribute
- href etiketini  # ile başlatmak
- id etiketi her html etiketi ile kullanılbilir
- aynı sayfada en üste çıkıp en alta indirir
```html
<h1 id="xxx">baslık</h1>

<a href="#xxx">git</a>
```
