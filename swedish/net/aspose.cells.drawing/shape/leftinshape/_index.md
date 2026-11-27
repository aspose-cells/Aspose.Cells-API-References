---
title: "Shape.LeftInShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar den horisontella förskjutningen av figuren från den vänstra kanten av föräldrafiguren i enheten 1/4000 av föräldrafigurens bredd"
type: docs
url: /sv/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet av 1/4000 av föräldraformens bredd.

```csharp
public int LeftInShape { get; set; }
```

### Anmärkningar

Gäller endast när denna form är i gruppen eller diagrammet.

### Exempel

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


