---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar och sätter det maximala radnumret för delad formel"
type: docs
url: /sv/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Hämtar och anger det maximala radnumret för delad formel.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Anmärkningar

Om numret är för stort fungerar autofiltret mycket långsamt i MS Excel 2013.

### Exempel

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
            
            // Sätt delad formel med 101 rader (överskrider MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Verifiera formeln i sista cellen
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Öka MaxRowsOfSharedFormula och testa igen i ett nytt blad
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

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


