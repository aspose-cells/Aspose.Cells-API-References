---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractFormulaChangeMonitor. L'evento che verrà attivato quando la formula in una cella viene modificata"
type: docs
url: /it/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

L'evento che verrà attivato quando la formula in una cella viene modificata.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | L'indice del foglio della cella modificata |
| rowIndex | Int32 | L'indice della riga della cella modificata |
| columnIndex | Int32 | L'indice della colonna della cella modificata |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza della nostra classe demo che eredita da AbstractFormulaChangeMonitor
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Imposta una formula in una cella per attivare la modifica
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Chiama OnCellFormulaChanged con indice foglio 0, riga 0, colonna 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Implementazione per gestire la modifica della formula
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Vedi anche

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


