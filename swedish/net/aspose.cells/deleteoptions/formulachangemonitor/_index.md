---
title: "DeleteOptions.FormulaChangeMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteOptions-egenskap. Hämtar/sätter övervakaren för att spåra ändringar som orsakas av borttagningen"
type: docs
url: /sv/net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

Hämtar/anger övervakaren för att spåra ändringar som orsakas av borttagningen.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ställ in testdata
            cells["A1"].Formula = "=A5";
            cells["A5"].Value = 10;
            
            // Lägg till villkorsstyrd formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");

            // Skapa och tilldela övervakare
            CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
            DeleteOptions options = new DeleteOptions
            {
                FormulaChangeMonitor = monitor,
                UpdateReference = true
            };

            // Ta bort rad som bör utlösa formelförändringar
            cells.DeleteRows(2, 1, options);

            // Skriv ut övervakningsresultat
            Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
            Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public bool CellChangesDetected { get; private set; }
        public bool FormatConditionChangesDetected { get; private set; }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            CellChangesDetected = true;
            Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
        }

        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            FormatConditionChangesDetected = true;
            Console.WriteLine("Format condition formula changed");
        }
    }
}
```

### Se även

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


