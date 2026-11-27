---
title: "ScenarioInputCell.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCell-egenskapen. Hämtar och anger inmatningscellens adress"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Hämtar och anger adressen för indatacellen.

```csharp
public string Name { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett scenario
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Hämta scenariot
            Scenario scenario = scenarios[scenarioIndex];

            // Lägg till indataceller till scenariot
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Hämta inmatningscellerna
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Demonstrera användning av Name‑egenskapen
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Verifiera att namnen matchar förväntade värden
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Se även

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


