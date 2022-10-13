- tablo içeriği row by row(satır-satır) oluşturulur.
- tr, satırları oluşturur
- td, her satırın hücrelerini olusturur
- th, td gibi sadece başlık için kullanılır
- bos hücre için yinede td,th olusturulmalı


```html
<table>

    <caption>veri datası</caption>

    <tr>

        <th scope="col">Name</th>

        <th scope="col">Age</th>

    </tr>

    <tr>

        <td>John Doe</td>

        <td>24</td>

      </tr>

      <tr>

        <td>Alice Doe</td>

        <td>54</td>

      </tr>

</table>
```
![[Pasted image 20220809194751.png]]

--> caption kullanma
--> herseyi figure içinde figcaption ile kullanma
--> table summary attr
--> p id'sini, table `aria-describedby` attribute ile kullanma(p yerine farklı etikette olur, acıklama içerir)

-> sekillendirme
```html
<table style="border: 1px solid black;">
```

- scope attr;
	- col, Hücrenin bir sütun için bir başlık olduğunu belirtir
	- row, Hücrenin bir satır için bir başlık olduğunu belirtir
	- colgroup, Hücrenin bir sütun grubu için bir başlık olduğunu belirtir
	- rowgroup, Hücrenin bir satır grubu için bir başlık olduğunu belirtir


### hücre birleştirme

```html
<td colspan="_number_">
<td rowspan="_number_">
<!-- th içinde geçerli  -->
```


### LONG Tables

```html
<table>  
<thead>  
  <tr>  
    <th>Month</th>  
    <th>Savings</th>  
    <th rowspan="3">Savings for holiday!</th>  
  </tr>  
</thead>  
<tbody>  
  <tr>  
    <td>January</td>  
    <td>$100</td>  
    <td rowspan="0">$100</td>  
  </tr>  
  <tr>  
    <td>February</td>  
    <td>$80</td>  
  </tr>  
</tbody>  
</table>
```


- cellpadding, cellspacing, width -- (px de/olarak yazılır)