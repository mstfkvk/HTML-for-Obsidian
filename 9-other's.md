#ID_atrribute
- uniquely identify
- global attribute, her element için kullanılır
- harf veya (\_)  ile başlar

#class_attribute
- global 
- class="a b" , 2 farklı value atanabilir

#block_element
- yeni satıra geçiren element
- h1, p, ul, li

#inline_element
- aynı satırda devam
- a, b, em, img


=> head elementi arasında direk css kullanımı
```html
<style type="text/css">

    body {
      background-color: #f5f5f5;
    }

</style>
```
=> css yolu belirtme, head içinde, type="text/css" gerek yok artık
```html
<link rel="stylesheet" href="style.css"  />
```



---

```html
<article>

      <header>

        <main></main>

        <nav></nav>

        <aside></aside>

      </header>

      <footer></footer>

    </article>

    <section></section>

    <hgroup><h1></h1><h2></h2></hgroup>
```


```html
<a href="...">
 <figure>
     <figcaption>name</figcaption>
     musty
  </figure>
</a>

<!-- figcaption, figure elementindeki içeriğin tanımını içerir -->

<!-- herseyi <a> etiketi içine alarak tıklanan her yazı ve resim için yönlendirme yapılabilir -->    
```

---


```html
<code>java</code> <br />

    <pre>

      <code>

        java

      js

    </code>

  </pre>

    <br />

    <var>variable name</var> <br />

    <kbd>keybord button, like cmd-ctrl</kbd> <br />

    <samp>output of the codes</samp>
```
![[Pasted image 20220822115507.png]]

---

-> other html elements

```html
<mark>mustafa</mark>

<small>kvk</small>
```
![[Pasted image 20220822120633.png]]
