---
title: "InsertOptions.FormulaChangeMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà InsertOptions. Ottiene/imposta il monitor per tracciare le modifiche causate dall'inserimento"
type: docs
url: /it/net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Ottiene/imposta il monitor per tracciare le modifiche causate dall'inserimento.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio con formule
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";
            worksheet.Cells["B1"].Formula = "=SUM(A1:A2)";

            try
            {
                // Crea un'istanza di InsertOptions
                InsertOptions options = new InsertOptions();

                // Crea un'implementazione personalizzata di FormulaChangeMonitor
                var monitor = new CustomFormulaChangeMonitor();
                options.FormulaChangeMonitor = monitor;

                // Visualizza il FormulaChangeMonitor corrente
                Console.WriteLine("FormulaChangeMonitor is set: " +
                    (options.FormulaChangeMonitor != null));

                // Inserisci righe che potrebbero attivare modifiche alle formule
                worksheet.Cells.InsertRows(1, 1, options);

                // Salva il risultato
                workbook.Save("FormulaChangeMonitorDemo.xlsx");
                Console.WriteLine("FormulaChangeMonitor demonstration completed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Implementazione personalizzata di AbstractFormulaChangeMonitor
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

### Vedi anche

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


