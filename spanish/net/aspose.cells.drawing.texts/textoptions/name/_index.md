---
title: "TextOptions.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Obtiene y establece el nombre de la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/name/
---
## TextOptions.Name property

Obtiene y establece el nombre de la forma.

```csharp
public override string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Demostrar el uso de la propiedad Name
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            textOptions.Color = System.Drawing.Color.Blue;
            
            workbook.Save("TextOptionsPropertyNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


