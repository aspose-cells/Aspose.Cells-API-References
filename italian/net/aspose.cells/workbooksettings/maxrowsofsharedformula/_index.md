---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta il numero massimo di righe della formula condivisa"
type: docs
url: /it/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Ottiene e imposta il numero massimo di righe della formula condivisa.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Osservazioni

Se il numero è troppo grande, l'autofiltro funziona molto lentamente in MS Excel 2013.

### Esempi

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
            
            // Imposta la formula condivisa con 101 righe (supera MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Verifica la formula nell'ultima cella
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Aumenta MaxRowsOfSharedFormula e testa di nuovo in un nuovo foglio
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

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


