---
title: "SolidFill.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SolidFill. Obtiene o establece el Color"
type: docs
url: /es/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Obtiene o establece el Color.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue una forma a la hoja de cálculo con los parámetros correctos
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Establezca propiedades de la forma con color
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Demuestre el uso de la propiedad Color
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Guarda el libro de trabajo
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


