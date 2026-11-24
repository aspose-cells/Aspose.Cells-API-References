---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions‑Eigenschaft. Gibt an, ob die Spaltenbreite in Zeichenbreiten kopiert wird"
type: docs
url: /de/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein Quell‑Arbeitsbuch mit Beispieldaten
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Setze die Spaltenbreite in Zeichen zur Demonstration
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Fügen Sie einige Beispieldaten hinzu
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopieren mit ColumnCharacterWidth auf true gesetzt
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Ergebnis speichern
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Zum Vergleich: Kopieren ohne ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


