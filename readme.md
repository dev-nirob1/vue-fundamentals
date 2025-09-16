# What is Vue.js?
- Vue.js is a progressive Javascript framework used to build user interfaces and single page applications (SPA). It is follows a component-base architecture making development modular and efficient.

# Why Vue.js?
-It is Progressive, Easy to learn, Lightweight and fast, Reactive, Component-Based and Great ecosystem. Perfect for building dynamic and maintainable web applications.

`𝘊𝘶𝘳𝘳𝘦𝘯𝘵𝘭𝘺 𝘦𝘹𝘱𝘭𝘰𝘳𝘪𝘯𝘨 𝘝𝘶𝘦.𝘫𝘴 𝘧𝘰𝘳 𝘣𝘶𝘪𝘭𝘥𝘪𝘯𝘨 𝘥𝘺𝘯𝘢𝘮𝘪𝘤 𝘸𝘦𝘣 𝘢𝘱𝘱𝘴!`


# 𝚠̲𝚑̲𝚊̲𝚝̲ ̲𝚒̲𝚜̲ ̲𝚁̲𝚎̲𝚏̲(̲)̲:̲
 ref() is a reactive value in Vue.js. It lets you track changes and automatically update the DOM, so you don’t need to manipulate it manually.

In plain JavaScript, when a variable changes, the DOM does not update by itself. You have to write something like:

``` document.getElementById('hashtag#id').innerText = value;
```
𝙴̲𝚡̲𝚊̲𝚖̲𝚙̲𝚕̲𝚎̲ ̲𝙹̲𝚊̲𝚟̲𝚊̲𝚜̲𝚌̲𝚛̲𝚒̲𝚙̲𝚝̲: 

```html
<p id="count">0</p>
<button onclick​="increase()">Increase</button>

<​script>
 let count = 0
 // increment function
 function increase() {
 count++
 document.getElementById('count').innerText = count
 }
<​/script>
```

# 𝙴̲𝚡̲𝚊̲𝚖̲𝚙̲𝚕̲𝚎̲ ̲𝚅̲𝚞̲𝚎̲.̲𝚓̲𝚜̲:
 ```<​script setup> 
import {ref} from 'vue'; 
const count = ref(0); 

//increament function 
function increase() { 
 count.value++;
 } 
<​/script> 
<template> 
 <div> 
 <p> current count: {{count}} </p>
 <button @click='increase'>Increase</button> 
 </div> 
</template>
```
Here, count starts at 0 and increase by one every time the button is clicked. In Javascript(logic), you need to update it with .value, but in template(HTML), you just use {{count}}.