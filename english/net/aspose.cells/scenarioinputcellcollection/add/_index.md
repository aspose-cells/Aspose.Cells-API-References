---
title: ScenarioInputCellCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ScenarioInputCellCollection method. Adds an input cell
type: docs
url: /net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Adds an input cell.

```csharp
public int Add(int row, int column, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index of input cell. |
| column | Int32 | The column index of input cell. |
| value | String | The value of input cell. |

### Examples

```csharp
// Called: inputCells.Add(0, 0, "10"); // Adding cell A1 with value 10
public static void ScenarioInputCellCollection_Method_Add()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a scenario to the worksheet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Access the ScenarioInputCellCollection
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Add input cells to the scenario
            inputCells.Add(0, 0, "10"); // Adding cell A1 with value 10
            inputCells.Add(1, 1, "20"); // Adding cell B2 with value 20

            // Access and print the properties of the ScenarioInputCellCollection
            Console.WriteLine("Capacity: " + inputCells.Capacity);
            Console.WriteLine("Count: " + inputCells.Count);

            // Access individual ScenarioInputCell by index
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Print details of the input cells
            Console.WriteLine($"Input Cell 1: Row={inputCell1.Row}, Column={inputCell1.Column}, Value={inputCell1.Value}");
            Console.WriteLine($"Input Cell 2: Row={inputCell2.Row}, Column={inputCell2.Column}, Value={inputCell2.Value}");

            // Save the workbook
            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
```

### See Also

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


