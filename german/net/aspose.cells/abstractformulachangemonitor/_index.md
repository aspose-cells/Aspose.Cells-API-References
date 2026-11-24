---
title: "Klasse AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AbstractFormulaChangeMonitor Klasse. Überwacht für den Benutzer die Änderung von Formeln während bestimmter Vorgänge"
type: docs
url: /de/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Überwacht für den Benutzer die Änderungen von Formeln während bestimmter Vorgänge.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | Das Ereignis, das ausgelöst wird, wenn die Formel in einer Zelle geändert wird. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | Das Ereignis, das ausgelöst wird, wenn die Formel einer FormatCondition geändert wird. |

### Hinweise

Zum Beispiel können beim Löschen/Einfügen eines Zellbereichs Formeln anderer Zellen aufgrund der Verschiebung von Verweisen geändert werden. Bitte beachten Sie, dass Methoden im Monitor mehrfach für ein Objekt aufgerufen werden können, das die Formel enthält.

### Beispiele

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
            
            // Setze einige Formeln in Zellen
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Füge Zeilen ein, die Formelländerungen auslösen
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


