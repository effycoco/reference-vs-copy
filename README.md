# Objects and Arrays - Reference VS Copy

A project from [JavaScript 30 -14](https://youtu.be/YnfwDQ5XYF4).

当将一个变量赋值给另一个变量时，是复制还是增加一个指针？取决于等号右边变量的数据类型，如果是数字、字符串、布尔值（原始类型），则复制；如果是数组和对象（object 类型，不包括函数），则增加指针而不复制，因此后续改变其中一个变量的值，另一个变量也会随之改变。（记忆时只要记住数字、字符串、布尔值类型的变量赋值给另一变量是复制，数组和对象变量赋值给另一变量是增加指针不复制）

那么如何复制数组呢？

1. `const array1=array0.slice()`
2. `const array2=[].concat(array0)`
3. `const array3=[...array0]`
4. `const array4=Array.from(array0)`

如何复制对象？

1. `const object1=Object.assign(object0)`
