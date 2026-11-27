---
title: "Klass AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AbstractFormulaChangeMonitor-klass. Övervakar för användaren att spåra förändringar av formler under vissa operationer"
type: docs
url: /sv/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Övervaka för att användaren ska kunna följa förändringar av formler under vissa operationer.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | Händelsen som utlöses när formeln i en cell ändras. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | Händelsen som utlöses när formeln för FormatCondition ändras. |

### Anmärkningar

Till exempel, när du tar bort/infogar ett cellområde kan formler i andra celler ändras på grund av referensförflyttning. Observera att metoder i övervakaren kan anropas flera gånger för ett objekt som innehåller formeln.

### Exempel

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
            
            // Ange några formler i celler
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Infoga rader som kommer att utlösa formelförändringar
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


