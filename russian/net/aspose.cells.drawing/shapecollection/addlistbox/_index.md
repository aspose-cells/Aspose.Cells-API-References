---
title: AddListBox
second_title: Справочник по Aspose.Cells для .NET API
description: Добавляет ListBox на рабочий лист.
type: docs
weight: 170
url: /ru/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Добавляет ListBox на рабочий лист.

```csharp
public ListBox AddListBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| top | Int32 | Представляет вертикальное смещение ListBox от его левой строки в единицах пикселей. |
| upperLeftColumn | Int32 | Индекс верхнего левого столбца. |
| left | Int32 | Представляет горизонтальное смещение ListBox от его левого столбца в единицах пикселей. |
| height | Int32 | Представляет высоту ListBox в пикселях. |
| width | Int32 | Представляет ширину ListBox в пикселях. |

### Возвращаемое значение

Объект ListBox.

### Примеры

```csharp

[C#]
  //добавляем список box
ListBox listBox = shapes.AddListBox(1, 0, 1, 0, 100, 50);
```

### Смотрите также

* class [ListBox](../../listbox)
* class [ShapeCollection](../../shapecollection)
* пространство имен [Aspose.Cells.Drawing](../../shapecollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->