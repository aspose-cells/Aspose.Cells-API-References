---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt den Typ der automatischen Anpassung der Zeilenhöhe zusammengeführter Zellen zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Liest und setzt den Typ der automatischen Anpassung der Zeilenhöhe zusammengeführter Zellen.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Hinweise

Excel ignoriert standardmäßig zusammengeführte Zellen beim Anpassen der Zeilenhöhe, sodass Aspose.Cells wie die Standardeinstellung von MS Excel funktioniert. Bitte setzen Sie diesen Typ, um die Art des automatischen Anpassen der Zeilenhöhe zusammengeführter Zellen zu ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen und Zellen zusammenführen
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // Zeilen automatisch anpassen mit AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Spalten automatisch anpassen mit AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


