---
title: "MsoLineFormat.ForeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Ottiene e imposta il colore di primo piano della linea di bordo"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Ottiene e imposta il colore di primo piano della linea del bordo.

```csharp
public Color ForeColor { get; set; }
```

### Esempi

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
            
            // Imposta le proprietà del formato linea includendo ForeColor
            textBox.LineFormat.ForeColor = Color.Red;
            textBox.LineFormat.Style = MsoLineStyle.Single;
            textBox.LineFormat.IsVisible = true;
            textBox.LineFormat.Weight = 2;

            workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
            
            // Verifica il colore salvato
            Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


