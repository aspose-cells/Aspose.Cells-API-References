---
title: "MsoLineFormat.ForeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MsoLineFormat propiedad. Obtiene y establece el color de primer plano de la línea del borde"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Obtiene y establece el color de primer plano de la línea del borde.

```csharp
public Color ForeColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            
            // Establecer propiedades de formato de línea incluyendo ForeColor
            textBox.LineFormat.ForeColor = Color.Red;
            textBox.LineFormat.Style = MsoLineStyle.Single;
            textBox.LineFormat.IsVisible = true;
            textBox.LineFormat.Weight = 2;

            workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
            
            // Verificar el color guardado
            Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


