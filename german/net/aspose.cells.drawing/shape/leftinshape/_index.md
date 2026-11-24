---
title: "Shape.LeftInShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz der Form von der linken Begrenzung der übergeordneten Form in Einheiten von 1/4000 der Breite der übergeordneten Form an"
type: docs
url: /de/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Breite der übergeordneten Form.

```csharp
public int LeftInShape { get; set; }
```

### Hinweise

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

### Beispiele

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


