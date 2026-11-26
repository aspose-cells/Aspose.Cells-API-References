---
title: "Class MsoLineFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.MsoLineFormat class. Representa el formato de líneas y puntas de flecha"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Representa el formato de línea y punta de flecha.

```csharp
public class MsoLineFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Obtiene y establece el color de fondo de la línea del borde. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Obtiene o establece el estilo de guión para la línea especificada. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Obtiene y establece el color de primer plano de la línea del borde. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Indica si el objeto es visible. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Devuelve un objeto Style que representa el estilo del rango especificado. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Devuelve o establece el grosor de la línea, en unidades de pt. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Instanciar un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de arco a la hoja de cálculo
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Obtener el objeto MsoLineFormat de la forma
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Establecer propiedades del objeto MsoLineFormat
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Guarda el libro de trabajo
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


