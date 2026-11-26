---
title: "Shape.TopInShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет вертикальное смещение фигуры от верхней границы родительской фигуры в единицах 1/4000 высоты родительской фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры.

```csharp
public int TopInShape { get; set; }
```

### Примечания

Применяется только когда эта фигура находится в группе или диаграмме.

### Примеры

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


