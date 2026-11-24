---
title: "HtmlSaveOptions.IgnoreInvisibleShapes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob nicht sichtbare Formen exportiert werden"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Gibt an, ob nicht sichtbare Formen exportiert werden sollen.

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

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
            // Arbeitsmappe mit einem Beispiel-Arbeitsblatt erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sichtbare und unsichtbare Formen hinzufügen
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            shape1.IsHidden = false;
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
            shape2.IsHidden = true;

            // Speichern mit IgnoreInvisibleShapes = true (Standard)
            HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
            saveOptions1.IgnoreInvisibleShapes = true;
            workbook.Save("output_ignore_invisible.html", saveOptions1);

            // Speichern mit IgnoreInvisibleShapes = false
            HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
            saveOptions2.IgnoreInvisibleShapes = false;
            workbook.Save("output_include_invisible.html", saveOptions2);

            Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


