---
title: ScenarioInputCellCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ScenarioInputCellCollection property. Gets ScenarioInputCell by index in the list
type: docs
url: /net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Gets [`ScenarioInputCell`](../../scenarioinputcell/) by index in the list.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The specific index in the list |

### Return Value

The [`ScenarioInputCell`](../../scenarioinputcell/) object

### Examples

```csharp
// Called: ScenarioInputCell inputCell1 = inputCells[0];
public static void ScenarioInputCellCollection_Property_Item()
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

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


