---
title: "Shape.TopInShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar det vertikala avståndet för formen från den övre kanten av föräldraformen i enhet av 1/4000 av föräldraformens höjd."
type: docs
url: /sv/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Representerar det vertikala avståndet för formen från den översta kanten på föräldraformen, i enhet av 1/4000 av föräldraformens höjd.

```csharp
public int TopInShape { get; set; }
```

### Anmärkningar

Gäller endast när denna form är i gruppen eller diagrammet.

### Exempel

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


