---
title: "ScenarioInputCell.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCell-Eigenschaft. Gibt die Adresse der Eingabezelle zurück und setzt sie"
type: docs
url: /de/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Liest und setzt die Adresse der Eingabezelle.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Szenario erstellen
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Das Szenario abrufen
            Scenario scenario = scenarios[scenarioIndex];

            // Füge Eingabezellen dem Szenario hinzu.
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Die Eingabezellen abrufen
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Überprüfen Sie, ob die Namen den erwarteten Werten entsprechen
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


