---
title: "Shape.TopInShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre en unidades de 1/4000 de la altura de la forma padre"
type: docs
url: /es/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre.

```csharp
public int TopInShape { get; set; }
```

### Observaciones

Solo se aplica cuando esta forma está en el grupo o gráfico.

### Ejemplos

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


