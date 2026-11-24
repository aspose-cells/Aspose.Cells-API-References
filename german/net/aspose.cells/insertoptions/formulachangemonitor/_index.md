---
title: "InsertOptions.FormulaChangeMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "InsertOptions Eigenschaft. Liest/Schreibt den Monitor zur Verfolgung von Änderungen, die durch das Einfügen verursacht werden"
type: docs
url: /de/net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Liest/setzt den Monitor zur Verfolgung von Änderungen, die durch das Einfügen verursacht werden.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten mit Formeln hinzu
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";
            worksheet.Cells["B1"].Formula = "=SUM(A1:A2)";

            try
            {
                // Erstelle eine InsertOptions-Instanz
                InsertOptions options = new InsertOptions();

                // Erstelle eine benutzerdefinierte Implementierung von FormulaChangeMonitor
                var monitor = new CustomFormulaChangeMonitor();
                options.FormulaChangeMonitor = monitor;

                // Zeige den aktuellen FormulaChangeMonitor an
                Console.WriteLine("FormulaChangeMonitor is set: " +
                    (options.FormulaChangeMonitor != null));

                // Zeilen einfügen, die Formelländerungen auslösen können
                worksheet.Cells.InsertRows(1, 1, options);

                // Ergebnis speichern
                workbook.Save("FormulaChangeMonitorDemo.xlsx");
                Console.WriteLine("FormulaChangeMonitor demonstration completed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Benutzerdefinierte Implementierung von AbstractFormulaChangeMonitor
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

### Siehe auch

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


