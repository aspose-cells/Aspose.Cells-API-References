---
title: "ScenarioInputCell.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCell-Eigenschaft. Gibt den Wert der Eingabezelle zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Liest und setzt den Wert der Eingabezelle.

```csharp
public string Value { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Szenario hinzufügen
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Eingabezellen mit Werten hinzufügen
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Werte zugreifen und ändern
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


