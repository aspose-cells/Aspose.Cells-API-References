---
title: "Klass Scenario"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Scenario-klass. Representerar ett enskilt scenario"
type: docs
url: /sv/net/aspose.cells/scenario/
---
## Scenario class

Representerar ett enskilt scenario.

```csharp
public class Scenario
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Hämtar och anger kommentaren för scenariot. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Hämtar inmatningscellerna för scenariot. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Anger om scenariot är dolt. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Anger om scenariot är låst för redigering när bladet är skyddat. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Hämtar och anger namnet på scenariot. |
| [User](../../aspose.cells/scenario/user/) { get; } | Hämtar namnet på den användare som senast ändrade scenariot. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Öppna scenariokollektionen för kalkylbladet
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Lägg till ett nytt scenario i samlingen
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Ställa in egenskaper för scenariot
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Öppna skrivskyddade egenskaper
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Spara arbetsboken
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


