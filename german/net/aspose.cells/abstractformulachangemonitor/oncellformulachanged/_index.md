---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractFormulaChangeMonitor-Methode. Das Ereignis, das ausgelöst wird, wenn die Formel in einer Zelle geändert wird"
type: docs
url: /de/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

Das Ereignis, das ausgelöst wird, wenn die Formel in einer Zelle geändert wird.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Der Blattindex der geänderten Zelle |
| rowIndex | Int32 | Der Zeilenindex der geänderten Zelle |
| columnIndex | Int32 | Der Spaltenindex der geänderten Zelle |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Instanz unserer Demo-Klasse, die von AbstractFormulaChangeMonitor erbt
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Setzen Sie eine Formel in einer Zelle, um die Änderung auszulösen
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Rufen Sie OnCellFormulaChanged mit Blattindex 0, Zeile 0, Spalte 0 (A1) auf
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Implementierung zur Handhabung von Formeländerungen
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Siehe auch

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


