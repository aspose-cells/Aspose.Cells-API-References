---
title: "HtmlSaveOptions.IgnoreInvisibleShapes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le forme non visibili"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Indica se esportare le forme non visibili

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIgnoreInvisibleShapesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con un foglio di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi forme visibili e invisibili
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            shape1.IsHidden = false;
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
            shape2.IsHidden = true;

            // Salva con IgnoreInvisibleShapes = true (predefinito)
            HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
            saveOptions1.IgnoreInvisibleShapes = true;
            workbook.Save("output_ignore_invisible.html", saveOptions1);

            // Salva con IgnoreInvisibleShapes = false
            HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
            saveOptions2.IgnoreInvisibleShapes = false;
            workbook.Save("output_include_invisible.html", saveOptions2);

            Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


