---
title: "ScenarioCollection.LastSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioCollection egenskap. Anger vilket scenario som senast valdes av användaren för att köras/visas"
type: docs
url: /sv/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Anger vilket scenario som senast valdes av användaren för att köras/visas.

```csharp
public int LastSelected { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till scenarier
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Ställ in aktivt scenario och senast valda indexet
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Verifiera och demonstrera LastSelected-egenskapen
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Ändra senast valda index
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Se även

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


