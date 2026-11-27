---
title: "Worksheet.Scenarios"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar samlingen av Scenario"
type: docs
url: /sv/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Hämtar samlingen av [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Lägg till scenarier
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Spara arbetsboken
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Rensa scenarier och spara igen
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


