---
title: Scenario.InputCells
second_title: Aspose.Cells for .NET API Reference
description: Scenario property. Gets the input cells of scenario
type: docs
url: /net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Gets the input cells of scenario.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Examples

```csharp
// Called: ScenarioInputCellCollection inputCells = scenario.InputCells;
public static void Property_InputCells()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a scenario to the worksheet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Add input cells to the scenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Accessing the input cells
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Displaying properties of the input cells
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Modify the value of the first input cell
            inputCell1.Value = "150";

            // Save the workbook
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
```

### See Also

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


