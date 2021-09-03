# dwiJs
lightweight javascript utilities function collections

## Instalation
1. using cdn (required internet)
   - put script tag in your index.html header

```html
<script src="https://cdn.jsdelivr.net/npm/dwijs@1.0.1/dist/dwiJs.js"></script>
```

2. or download [dwiJs.rar](https://github.com/ZiddanDwiPutra/dwijs/blob/main/dwiJs.rar) file
   - extract rar file to folder /src
   - and then put script tag in your index.html header

```html
<script src="src/dwiJs.js"></script>
```

## Usage
Access all Utils easily
(Read [Documentations](https://ziddandwiputra.github.io/dwijs-docs) for detail)

```javascript
// Access StringUtils
StringUtils.join();

// Access EvalUtils
EvalUtils.containsArray("objArr[0]");

// and much more
StringUtils, EvalUtils, NumberUtils, ArrayUtils, ObjectUtils, ElementUtils
```
## DwiVar for modeling variables

```html
<div class="app">
   <span> {{text}} </span>
</div>
<script>
   // init DwiVar 
   new dwi.var("app", {
      data: (){
         return {
            text: "your text here"
         }
      }
   });
</script>
```

```html
<div class="app">
   <div> {{text}} </div>
   <div>
      Change Text Here : <br>
      <input model value="{{text}}"> 
   </div>
</div>
<script>
   // init DwiVar 
   let app = new dwi.var(".app", {
      data: (){
         return {
            text: "write text"
         }
      }
   });
</script>
```
