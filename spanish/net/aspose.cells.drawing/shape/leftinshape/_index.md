---
title: "Shape.LeftInShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre en unidades de 1/4000 del ancho de la forma padre"
type: docs
url: /es/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre, en unidades de 1/4000 del ancho de la forma padre.

```csharp
public int LeftInShape { get; set; }
```

### Observaciones

Solo se aplica cuando esta forma está en el grupo o gráfico.

### Ejemplos

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


