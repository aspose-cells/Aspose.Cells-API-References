---
title: "Scenario.Comment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario-egenskap. Hämtar och anger kommentaren för scenariot"
type: docs
url: /sv/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Hämtar och anger kommentaren för scenariot.

```csharp
public string Comment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en scenariokollektion
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Lägg till ett scenario
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Ställ in scenario-egenskaper
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Lägg till inmatningsceller i scenariot med cellreferenser och värden
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Visa scenario-kommentar
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Spara arbetsboken
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


