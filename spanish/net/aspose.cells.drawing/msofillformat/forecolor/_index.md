---
title: "MsoFillFormat.ForeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormat. Obtiene y establece el color de primer plano del relleno"
type: docs
url: /es/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Obtiene y establece el color de primer plano del relleno.

```csharp
public Color ForeColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Obtener el formato de relleno
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Establece y demuestra la propiedad ForeColor
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Modifica el ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Guarda el libro de trabajo
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


