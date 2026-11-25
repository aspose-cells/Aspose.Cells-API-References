---
title: "Classe AbstractFormulaChangeMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractFormulaChangeMonitor. Monitor per l'utente per tenere traccia delle modifiche delle formule durante determinate operazioni"
type: docs
url: /it/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Monitor per l'utente per tenere traccia delle modifiche delle formule durante determinate operazioni.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | L'evento che verrà attivato quando la formula in una cella viene modificata. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | L'evento che verrà attivato quando la formula di FormatCondition viene modificata. |

### Osservazioni

Ad esempio, durante l'eliminazione/inserimento di un intervallo di celle, le formule di altre celle possono essere modificate a causa dello spostamento dei riferimenti. Si prega di notare che i metodi nel monitor possono essere invocati più volte per un singolo oggetto che contiene la formula.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Imposta alcune formule nelle celle
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Inserisci righe che attiveranno modifiche alle formule
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


