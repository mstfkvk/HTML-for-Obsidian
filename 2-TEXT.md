### headings

```html
<h1> main heading </h1>
<h2> sub heading  </h2>
..
<h6> ....         </h6>
```

###  paragraphs

```html
<p>   </p>
```
- ardısık paragraflar arasında belirgin boşlukşat bırakır

### bold & italic

```html
<b>  </b>
<i>  </i>
```

### superscript

```html
4<sup> th </sup>    
```

### subscript

```html
H<sub> 2 </sub>O
```

![[Pasted image 20220805195011.png]]

> [! note]
> white space ; browser 2 veya daha fazla boşlugu tek bosluk olarak gösterir.


### line breaks & horizontal rules

<mark class="hltr-green">Empty element</mark> , denir bu tür elementlere - acılıs kapanıs tagleri yoktur.

```html
<br/>    <!-- alt satırdan devem eder-->
<hr/>    <!-- yatay çizgi çizer-->
```

### semantic markup
- anlamsa biçimlendirme
- screen reader vurgulayarak okur
- search engine

```html

<strong> </strong>  <!-- kalın vurgu --> <!-- kalın yazar -->

<em>  </em>         <!-- ince vurgu --> <!-- eğik yazar -->

<blockquote cite="https://..."> siteden alıntı yapar </blockquote>  <!-- satırbası yapar düz yazı olarak  --> <!-- BLOCK ELEMENT -->

<q>   <q/>  <!-- inline element bu, cıktısı tırnak içinde -->

<abbr title="abbreviation - kısaltma"> abbr </abbr> 

<cite> eserden alıntı </cite>    <!-- italic gosterir -->

<dfn> </dfn>     <!-- italic gösterir, bazı browserlar da duz-aynı -->

```

![[Pasted image 20220805201531.png]]
![[Pasted image 20220805201707.png]]


### author detail
- specific kullanımı vardır, yazarla ilgili detaylar içerir.
- hcard olarak bilinip kullanılır.

```html
<adress>   </adress>  <!-- italic gösterir -->
```

### changes to content

```html
<del>  </del>   <!-- ortadan üstünü çizer --> 

<ins>  </ins>   <!-- altını çizer --> 

<s> </s>        <!-- del'in aynısı -->

<u> </u>        <!-- altını çizer -->
```
![[Pasted image 20220805203045.png]]
![[Pasted image 20220805203104.png]]

