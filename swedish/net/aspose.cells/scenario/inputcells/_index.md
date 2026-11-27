---
title: "Scenario.InputCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario‑egenskap. Hämtar inmatningscellerna för scenariot"
type: docs
url: /sv/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Hämtar inmatningscellerna för scenariot.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario i kalkylbladet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till inmatningsceller i scenariot med egenskapen InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Ändra värdet på den första inmatningscellen
            inputCells[0].Value = "150";

            // Spara arbetsboken
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


