# CSS Position ក្នុង CSS

`position` គឺជា property មួយក្នុង CSS ដែលប្រើសម្រាប់កំណត់ទីតាំង (position) របស់ element នៅលើ webpage។

## Syntax

```css
selector {
  position: value;
}
```

## ប្រភេទនៃ Position

### 1. static (Default)

`static` គឺជា default value របស់ element ទាំងអស់។
Element នឹងបង្ហាញតាមលំដាប់ធម្មតា (normal flow)។

```css
.box {
  position: static;
}
```

### 2. relative

`relative` អនុញ្ញាតឲ្យ element ផ្លាស់ទីពីទីតាំងដើមរបស់វា ដោយប្រើ `top`, `right`, `bottom`, `left`។

```css
.box {
  position: relative;
  top: 20px;
  left: 30px;
}
```

### 3. absolute

`absolute` ធ្វើឲ្យ element ចេញពី normal flow ហើយកំណត់ទីតាំងដោយផ្អែកលើ parent ដែលមាន `position` មិនមែន `static`។

```css
.box {
  position: absolute;
  top: 50px;
  right: 20px;
}
```

### 4. fixed

`fixed` ធ្វើឲ្យ element នៅជាប់ទីតាំងដដែល ទោះបី scroll page ក៏ដោយ។

```css
.box {
  position: fixed;
  bottom: 10px;
  right: 10px;
}
```

### 5. sticky

`sticky` គឺជាការលាយរវាង `relative` និង `fixed`។
Element នឹង scroll ជាមួយ page រហូតដល់ចំណុចកំណត់។

```css
.box {
  position: sticky;
  top: 0;
}
```

# Position Properties

| Property | អត្ថន័យ               |
| -------- | --------------------- |
| top      | កំណត់ចម្ងាយពីខាងលើ    |
| right    | កំណត់ចម្ងាយពីខាងស្តាំ |
| bottom   | កំណត់ចម្ងាយពីខាងក្រោម |
| left     | កំណត់ចម្ងាយពីខាងឆ្វេង |

# Example

```html
<div class="container">
  <div class="box">Hello CSS</div>
</div>
```

```css
.container {
  position: relative;
  width: 300px;
  height: 200px;
  background: lightgray;
}

.box {
  position: absolute;
  top: 20px;
  left: 50px;
  background: blue;
  color: white;
  padding: 10px;
}
```

# សេចក្ដីសន្និដ្ឋាន

CSS `position` ជួយឲ្យយើងគ្រប់គ្រងទីតាំង element បានយ៉ាងងាយស្រួល។
ការយល់ដឹងអំពី `static`, `relative`, `absolute`, `fixed`, និង `sticky` គឺសំខាន់សម្រាប់ការរចនា website។
