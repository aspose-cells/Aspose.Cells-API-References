---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die maximale Zeilenzahl der gemeinsam genutzten Formel zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Liest und setzt die maximale Zeilennummer der geteilten Formel.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Hinweise

Wenn die Zahl zu groß ist, arbeitet der Autofilter in MS Excel 2013 sehr langsam.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Setze eine gemeinsame Formel mit 101 Zeilen (überschreitet MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Überprüfe die Formel in der letzten Zelle
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Erhöhe MaxRowsOfSharedFormula und teste erneut in einem neuen Blatt
            book.Settings.MaxRowsOfSharedFormula = 1024;
            Worksheet sheet2 = book.Worksheets.Add("Sheet2");
            cells = sheet2.Cells;
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
            
            book.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


