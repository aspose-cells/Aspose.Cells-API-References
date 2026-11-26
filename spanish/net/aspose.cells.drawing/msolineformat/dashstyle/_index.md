---
title: "MsoLineFormat.DashStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Obtiene o establece el estilo de guión para la línea especificada"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Obtiene o establece el estilo de guión para la línea especificada.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una forma para demostrar DashStyle
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Establecer propiedades de línea
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // Demostrar diferentes estilos de guión
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // Agregar otra forma con un estilo de guión diferente
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // Guarda el libro de trabajo
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


