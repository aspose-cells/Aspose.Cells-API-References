---
title: "InsertOptions.FormulaChangeMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "InsertOptions egenskap. Hämtar/sätter övervakaren för att spåra ändringar som orsakas av infogningen"
type: docs
url: /sv/net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Hämtar/anger övervakaren för att spåra ändringar som orsakas av infogningen.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med formler
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";
            worksheet.Cells["B1"].Formula = "=SUM(A1:A2)";

            try
            {
                // Skapa en InsertOptions-instans
                InsertOptions options = new InsertOptions();

                // Skapa en anpassad FormulaChangeMonitor-implementation
                var monitor = new CustomFormulaChangeMonitor();
                options.FormulaChangeMonitor = monitor;

                // Visa den aktuella FormulaChangeMonitor
                Console.WriteLine("FormulaChangeMonitor is set: " +
                    (options.FormulaChangeMonitor != null));

                // Infoga rader som kan utlösa formelförändringar
                worksheet.Cells.InsertRows(1, 1, options);

                // Spara resultatet
                workbook.Save("FormulaChangeMonitorDemo.xlsx");
                Console.WriteLine("FormulaChangeMonitor demonstration completed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Anpassad implementation av AbstractFormulaChangeMonitor
        private class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
        {
            public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
            {
                Console.WriteLine($"Formula changed at Sheet {sheetIndex}, Cell {rowIndex},{columnIndex}");
            }

            public override void OnFormatConditionFormulaChanged(FormatCondition fc)
            {
                Console.WriteLine($"Format condition formula changed: {fc.Formula1}");
            }
        }
    }
}
```

### Se även

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


