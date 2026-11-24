---
title: "ScenarioInputCell.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCell-Eigenschaft. Gibt den Zeilenindex der Eingabezelle zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Liest und setzt den Zeilenindex der Eingabezelle.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
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

            // Zugriff auf und Demonstration der Row-Eigenschaft
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Füge eine neue Zelle in Zeile 2 hinzu, anstatt zu versuchen, die vorhandene zu ändern
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


