---
title: "Shape.LeftInShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma genitore in unità di 1/4000 della larghezza della forma genitore"
type: docs
url: /it/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma genitore, in unità di 1/4000 della larghezza della forma genitore.

```csharp
public int LeftInShape { get; set; }
```

### Osservazioni

Si applica solo quando questa forma è nel gruppo o nel grafico.

### Esempi

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


