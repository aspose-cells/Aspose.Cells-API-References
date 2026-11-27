---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractFormulaChangeMonitor-metod. Händelsen som utlöses när formeln i en cell ändras"
type: docs
url: /sv/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

Händelsen som utlöses när formeln i en cell ändras.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Bladindex för den ändrade cellen |
| rowIndex | Int32 | Radindex för den ändrade cellen |
| columnIndex | Int32 | Kolumnindex för den ändrade cellen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av vår demoklass som ärver från AbstractFormulaChangeMonitor
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Ange en formel i en cell för att utlösa förändringen
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Anropa OnCellFormulaChanged med bladindex 0, rad 0, kolumn 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Implementering för att hantera formelförändring
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Se även

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


