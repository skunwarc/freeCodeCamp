---
title: To List
localeTitle: 列表
---# ToList

给定DataSet查询生成List。

### 签名

```csharp
Enumerable.ToList<TSource> Method (IEnumerable<TSource>) 
```

## 例

```csharp
var fruits = new List<Fruit>() { 
    new Fruit() { Id = 1, Name = "Orange",     Color = "Orange", Quantity: 3   }, 
    new Fruit() { Id = 2, Name = "Strawberry", Color = "Red",    Quantity: 12  }, 
    new Fruit() { Id = 3, Name = "Grape",      Color = "Purple", Quantity: 25  }, 
    new Fruit() { Id = 4, Name = "Pineapple",  Color = "Yellow", Quantity: 1   }, 
    new Fruit() { Id = 5, Name = "Apple",      Color = "Red",    Quantity: 5   }, 
    new Fruit() { Id = 6, Name = "Mango",      Color = "Yellow", Quantity: 2   } 
 }; 
 
 // Generates list of fruits name 
 var fruitsNames = fruits.Select(f => f.Name).ToList(); // { "Orange", "Strawberry", "Grape", "Pineapple", "Apple", "Mango" } 

```