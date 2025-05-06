---
title: ScenarioInputCell.Row
second_title: Aspose.Cells for .NET API Reference
description: ScenarioInputCell property. Gets and sets the row index of the input cell
type: docs
url: /net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Gets and sets the row index of the input cell.

```csharp
public int Row { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($&amp;quot;Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}&amp;quot;);
public static void Property_Row()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a scenario to the worksheet
            int scenarioIndex = worksheet.Scenarios.Add(&quot;Scenario 1&quot;);
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Add input cells to the scenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, &quot;100&quot;); // Adding cell A1 with value 100
            inputCells.Add(1, 1, &quot;200&quot;); // Adding cell B2 with value 200

            // Accessing the input cells
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Displaying properties of the input cells
            Console.WriteLine($&quot;Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}&quot;);
            Console.WriteLine($&quot;Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}&quot;);

            // Modify the value of the first input cell
            inputCell1.Value = &quot;150&quot;;

            // Save the workbook
            workbook.Save(&quot;ScenarioInputCellExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


