## Что такое и зачем нужна деструктуризация

- разбивка сложной структуры(массив,обьект ) на простые части в виде отдельных переменных;
```js
const cats = ['Mura','Pusha','Vasia','Pusia'];

const [cat1,cat2,cat3,cat4] = cats // на каждый элемент массива создается переменная куда записывается значение элемента

// аналогично как если бы мы создали переменную сonst cat1 = 'Mura' const cat2 = 'Pusha'

console.log(cat1) // Mura

console.log(cat3)// Vasia 



```



- получение  отдельных  элементов  из массивов или объектов без обьявления лишних переменных;


```js
const numbers = ["one", "two", "three"];

// без деструктурирования
const one = foo[0];
const two = foo[1];
const three = foo[2];

// с деструктурированием
const [one, two, three] = foo;




```

- управлять вложенными структурами, используя  синтаксис вложенной деструктуризации.

```js

const metadata = {
    title: "Scratchpad",
    translations: [
       {
        locale: "de",
        localization_tags: [ ],
        last_edit: "2014-04-14T08:43:37",
        url: "/de/docs/Tools/Scratchpad",
        title: "JavaScript-Umgebung"
       }
    ],
    url: "/en-US/docs/Tools/Scratchpad"
};

const { title: englishTitle, translations: [{ title: localeTitle }] } = metadata;


```
