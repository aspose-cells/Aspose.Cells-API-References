---
title: "ScenarioInputCell.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCell-Eigenschaft. Liest und setzt den Spaltenindex der Eingabezelle."
type: docs
url: /de/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Liest und setzt den Spaltenindex der Eingabezelle.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Szenario dem Arbeitsblatt hinzu.
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Füge Eingabezellen dem Szenario hinzu.
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Zugriff auf und Demonstration der Column-Eigenschaft
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Da Column schreibgeschützt ist, müssen wir das Element entfernen und erneut hinzufügen, um die Spalte zu ändern
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Die Änderung überprüfen
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


