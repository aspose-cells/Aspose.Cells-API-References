---
title: GetLinkedCell
second_title: Справочник по Aspose.Cells для .NET API
description: Получает диапазон связанный со значением элемента управления.
type: docs
weight: 1050
url: /ru/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Получает диапазон, связанный со значением элемента управления.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу по локали. |

### Возвращаемое значение

Диапазон, связанный со значением элемента управления.

### Примеры

```csharp

[C#]
//Вы можете получить такие результаты, как '$A$1'
string link = shape.GetLinkedCell(false, false);
```

### Смотрите также

* class [Shape](../../shape)
* пространство имен [Aspose.Cells.Drawing](../../shape)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
