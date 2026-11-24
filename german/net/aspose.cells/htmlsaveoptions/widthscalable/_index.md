---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. Der Standardwert ist false.

```csharp
public bool WidthScalable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // HTML‑Speicheroptionen mit WidthScalable‑Eigenschaft festlegen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Mit skalierbarer Breite speichern
            workbook.Save("output_scalable.html", options);
            
            // Erneut mit fester Breite speichern
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


