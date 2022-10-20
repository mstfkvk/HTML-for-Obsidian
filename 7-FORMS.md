> aria-label, ekranda görünür olmayan metin etiketlerinin tanımlanmasında
> aria-labelledby, ekranda görünür olan metinlerin tanımlanmasında kullanılır


```html 
<form action="http://localhost:8080/index" method="post">
<!-- 
action: sayfa URL'sini içerir


method: 
get-> serverdan geri alınacak bilgiler için kullanılır(default)
post-> hassas veri içeriyorsa, kullanıcı dosya ekleyecekse, veri tabanına veri eklenip-silinecekse
dialog-> form <dialog> elementi içindeyse submit edildiğinde dialog'u kapatır
-->
</form>
```
 
-----

```html
<!-- IMPLICIT LABEL (not recommended for use) - the label wraps the input. -->
<label> 
  Name:
  <input type="text" name="name" />
</label>

<!-- EXPLICIT LABEL (recommended for use) - the label is connected to an input via "for" and "id" -->
<label for="explicit-label-name">Name: </label>
<input type="text" id="explicit-label-name" name="name" />

<!-- veya aria-label' lar kullanılır -->
```


# 7.1 ADDING TEXT

### text input
-> tek satırlık veri girişi
-> type bos bırakılırsa default olarak bu gecerli olur

```html
<span>username: </span>

<input type="text" name="username" maxlength="10" size="50">
```
![[Pasted image 20220821224253.png]]

### password input
-> text ile aynı sadece yazılar gizlidir-güvenilirlik yok
-> SSL, secure sockets layer

```html
<span>password: </span>

   <input type="password" name="sifre" size="10" maxlength="20" id="">
```
![[Pasted image 20220821224540.png]]

### text area

```html
<p>NOT empty element: </p>

<textarea name="comment" id="comment" cols="30" rows="3"></textarea>
```
![[Pasted image 20220821225416.png]]


# 7.2 MAKİNG CHOICES

### radio buttons
-> o 'nu olusturur sadece
-> value'lar farklı olmalı ve name' deki sorunun cevabıdır
```html
<span>What is the capital city of the Turkey? </span> <br>

<input type="radio" name="capital_city" value="malatya" id="" checked>malatya <br>

<input type="radio" name="capital_city" value="istanbul" id="">istanbul <br>

<input type="radio" name="capital_city" value="istanbul" id="">ankara <br>
```
![[Pasted image 20220821230242.png]]

### check boxes
-> 1' den fazla cevap secim ve gönderimi için kullanılır

```html
<!-- create checkbox example -->

    <div class="checkbox-example">

      <h2>Checkbox Example</h2>

      <input type="checkbox" id="checkbox-1" />

      <label for="checkbox-1">Checkbox 1</label>

      <input type="checkbox" id="checkbox-2" />

      <label for="checkbox-2">Checkbox 2</label>

      <input type="checkbox" id="checkbox-3"  checked/>

      <label for="checkbox-3">Checkbox 3</label>

    </div>
```
![[Pasted image 20220821230737.png]]


### drop-down boxes
-> label(kapsayıcı olacak sekilde)-select, for-id seklinde de olusturulabilir
-> size="3"  kac option gösterilcek
-> name=" "  formun adını bildirir

```html
    <!-- create dropdown listbox -->

    <select id="listbox" name="digit" >

      <option value="1">1</option>

      <option value="2">2</option>

      <option value="3">3</option>

      <option value="4">4</option>

      <option value="5">5</option>

      <option value="6">6</option>

      <option value="7">7</option>

      <option value="8">8</option>

      <option value="9">9</option>

      <option value="10">10</option>

    </select>
```
![[Pasted image 20220821230926.png]]


# 7.3 SUBMİTTİNG FORMS

### submit buttons

```html
<!-- create submitting button-->

<input type="submit" value="Submit" name="submit" />
```
![[Pasted image 20220821232625.png]]
	 
### image buttons

```html
<!-- create image button-->

<input type="image" src="images/create.png" alt="Create2" onclick="create()" />
```
![[Pasted image 20220822015020.png]]


# 7.4 UPLOADİNG FİLES

### file upload
-> method="post" zorunlu

```html
 <!-- create file upload -->

<form action="upload.php" method="post" enctype="multipart/form-data">

dosyalari seçiniz:

<input type="file" name="file" /> <br>

dosyalari yükle:  

<input type="submit" value="Upload" />

</form>
```
![[Pasted image 20220821232153.png]]

--- 

# EXTRA's

-> button etiketi içine resim(<img>) ve text beraber eklenebilir

```html
<button>
    <img src="images/create.png" alt="create" />

    <span> add </span>
</button>
```
![[Pasted image 20220822093259.png]]

-> button cesitleri

```html
<button type="submit">submit-1</button>

   <button type="reset">reset-2</button>

   <button disabled="disabled">disabled-3</button>
```
![[Pasted image 20220822093459.png]]


-> input-hidden webpage sahibi için kullanıcı göremez

```html
  <input type="hidden" name="hidden">
```

-> Date, Email, URL, Search

```html
<input type="date" name="date" id=""> <br>
<input type="datetime" name="datetime" id=""> <br>
<input type="datetime-local" name="d.time-local" id=""> <br>
<input type="time" name="time" id=""> <br>

 --- <br>

<input type="email" name="mail" id=""> <br>
<input type="url" name="url" id=""> <br>
<input type="search" name="search" id=""> <br>

--- <br>

<input type="tel" name="tel" id=""> <br>
<input type="number" name="number" id=""> <br>

--- <br>

<input type="range" name="range" id=""> <br>
<input type="color" name="color" id=""> <br>
```

![[Pasted image 20220822095504.png]]

--- 

# Some attributes
1) The input `value` attribute specifies an initial value for an input field
2) The input `readonly` attribute specifies that an input field is read-only, cannot be modified, The <u>value</u> of a read-only input field will be sent when submitting the form!
3) The input `disabled` attribute, is unusable and un-clickable, The value of a disabled input field will not be sent when submitting the form!
4) The input `min` and `max` attributes work with number, range, date, datetime-local, month, time and week
5) The input `multiple` attribute specifies that the user is allowed to enter more than one value in an input field.email, and file
6) The input `placeholder` attribute specifies a short hint that describes the expected value of an input field
7) The input `required` attribute specifies that an input field must be filled out before submitting the form
8) The input `autofocus` attribute specifies that an input field should automatically get focus when the page loads.
9) The input `list` attribute refers to a `<datalist>` element that contains pre-defined options for an <input> element.
```html
<form>  
  <input list="browsers">  
  <datalist id="browsers">  
    <option value="Internet Explorer">  
    <option value="Firefox">  
    <option value="Chrome">  
    <option value="Opera">  
    <option value="Safari">  
  </datalist>  
</form>
```
![[Pasted image 20220822100953.png]]
10) The input `autocomplete` attribute specifies whether a form or an input field should have autocomplete on or off, Autocomplete allows the browser to predict the value. When a user starts to type in a field





# Grouping Form Elements

```html
<fieldset>

  <legend>mk</legend>

 </fieldset>
```
![[Pasted image 20220822093942.png]]

