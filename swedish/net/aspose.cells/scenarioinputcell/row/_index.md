---
title: "ScenarioInputCell.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCell-egenskapen. Hämtar och anger radindex för inmatningscellen"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Hämtar och anger radindex för indatacellen.

```csharp
public int Row { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario i kalkylbladet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till indataceller till scenariot
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Kom åt och demonstrera Row-egenskapen
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Lägg till en ny cell på rad 2 istället för att försöka ändra den befintliga
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Spara arbetsboken
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


