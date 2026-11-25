---
title: "Shape.TopInShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore in unità di 1/4000 dell'altezza della forma genitore"
type: docs
url: /it/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Rappresenta lo spostamento verticale della forma dal bordo superiore della forma padre, in unità di 1/4000 dell'altezza della forma padre.

```csharp
public int TopInShape { get; set; }
```

### Osservazioni

Si applica solo quando questa forma è nel gruppo o nel grafico.

### Esempi

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


