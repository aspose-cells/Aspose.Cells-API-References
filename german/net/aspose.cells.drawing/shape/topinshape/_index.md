---
title: "Shape.TopInShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Abstand der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form an."
type: docs
url: /de/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Höhe der übergeordneten Form.

```csharp
public int TopInShape { get; set; }
```

### Hinweise

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

### Beispiele

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


