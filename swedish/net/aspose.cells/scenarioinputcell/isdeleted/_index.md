---
title: "ScenarioInputCell.IsDeleted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCell-egenskapen. Anger om inmatningscellen är raderad"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Anger om indatacellen är borttagen.

```csharp
public bool IsDeleted { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till inmatningsceller
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Kom åt och visa inmatningsceller
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Ta bort den första inmatningscellen
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Spara arbetsboken
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


