---
title: Item
second_title: Справочник по Aspose.Cells для .NET API
description: Получает объект формы по указанному индексу.
type: docs
weight: 10
url: /ru/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Получает объект формы по указанному индексу.

```csharp
public Shape this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| index |  |

### Примеры

```csharp

[C#]
  //получить shape
Shape shape = shapes[shapes.Count -1];
```

### Смотрите также

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* пространство имен [Aspose.Cells.Drawing](../../shapecollection)
* сборка [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Получает объект фигуры по изображению фигуры

```csharp
public Shape this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name |  |

### Примеры

```csharp

[C#]
  //добавляем shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
  //получить shape
Shape shape1 = shapes["Rectangle 1"];
if(shape1 != null)
{
      // Получили фигуру с именем «Прямоугольник 1».
}
```

### Смотрите также

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* пространство имен [Aspose.Cells.Drawing](../../shapecollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
