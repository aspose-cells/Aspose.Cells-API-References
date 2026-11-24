---
title: "StyleFlag.ShrinkToFit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung 'Shrink to fit' wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Die Einstellung 'Verkleinern, um anzupassen' wird angewendet.

```csharp
public bool ShrinkToFit { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze Beispieldaten in eine Zelle
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Erstelle einen Stil mit aktiviertem ShrinkToFit
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Erstelle ein StyleFlag und aktiviere das ShrinkToFit-Flag
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Wenden Sie den Stil auf den Zellbereich an (explizit unter Verwendung von Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Spaltenbreite festlegen, um das Schrumpfen zu demonstrieren
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


