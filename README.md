# Yoga.JS
###Javascript library which powers javascript

Why Yoga? In Vedic Sanskrit, yoga (from the root yuj) means "to add", "to join", "to unite", or "to attach" in its most common literal sense. There are very many compound words containing yoga in Sanskrit. Yoga can take on meanings such as "connection", "contact", "union", "method", "application", "addition" and "performance". In simpler words, Yoga also means "combined".

In that sense, Yoga.JS make **connection** with existing Java objects like Array, Object, String, Math etc and provides methods in **addition** to what JS engine by default provides.

Many libraries are available which gives similar functionality to what Yoga.JS provides. But all libraries provides functions in different scope which requires more parameters more code. Yoga.JS powers javascript objects by adding methods to existing objects as if it supports by default by the javascript engine.

##Examples

## Array Concat

```
var a = [10, 20, 30];
var b = [40, 50, 60];

a.concat(b);
```

## Array Iterator

```
var a = [10, 20, 30];

a.iterator();
while(a.hasNext()){
    console.log(a.next());
}
```

## Array apply()

```
function square(n){ return n*n; }

var a = [10, 20, 30];

a.apply(square);

//Result: [100, 400, 900]

```

##Array Truthy

```
var a = [10, 0, 30, true, false];

a.truthy()

//Result: [10,30,true]
```

##Array Difference

```
var a = [10, 20, 30];
var b = [10, 40, 30];

a.difference(b)

//[20,40]
```

## Object size

```
var a = {a:1, b:2, c:3}

a.size()

//3
```

## Object Entries

```
var a = { foo: "bar", baz: 42 };
a.entries();

//Result:  [ ['foo', 'bar'], ['baz', 42] ]
```

## Function memoize

```
function add(a,b,c){return a + b + c;}

var madd = add.memoize()

madd()
```

## Window isArray

```
isArray({}) //false
isArray([]) //true
```

## Window isObject

```
isObject([]) //false

isObject({}) //true

```

### Authors and Contributors
Author: Vaseem Abbas Mohammed

### Suggestions/Issues
[Click here for Suggestions/Issues](https://github.com/vaseems/yoga.js/issues)
