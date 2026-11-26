---
title: "Shape.LeftInShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры.

```csharp
public int LeftInShape { get; set; }
```

### Примечания

Применяется только когда эта фигура находится в группе или диаграмме.

### Примеры

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


