---
title: ScenarioCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ScenarioCollection property. Gets the Scenario object by the index
type: docs
url: /net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Gets the [`Scenario`](../../scenario/) object by the index.

```csharp
public Scenario this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The specific index in the list. |

### Examples

```csharp
// Called: Scenario scenario = worksheet.Scenarios[scenarioIndex];
public static void Property_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a scenario to the worksheet
            int scenarioIndex = worksheet.Scenarios.Add(&quot;Scenario1&quot;);
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Access the ScenarioInputCellCollection
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Add input cells to the scenario
            inputCells.Add(0, 0, &quot;10&quot;); // Adding cell A1 with value 10
            inputCells.Add(1, 1, &quot;20&quot;); // Adding cell B2 with value 20

            // Access and print the properties of the ScenarioInputCellCollection
            Console.WriteLine(&quot;Capacity: &quot; + inputCells.Capacity);
            Console.WriteLine(&quot;Count: &quot; + inputCells.Count);

            // Access individual ScenarioInputCell by index
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Print details of the input cells
            Console.WriteLine($&quot;Input Cell 1: Row={inputCell1.Row}, Column={inputCell1.Column}, Value={inputCell1.Value}&quot;);
            Console.WriteLine($&quot;Input Cell 2: Row={inputCell2.Row}, Column={inputCell2.Column}, Value={inputCell2.Value}&quot;);

            // Save the workbook
            workbook.Save(&quot;ScenarioInputCellCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


