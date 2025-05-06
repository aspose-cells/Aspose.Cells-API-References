---
title: ConditionalFormattingCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection method. Adds a FormatConditions to the collection
type: docs
url: /net/aspose.cells/conditionalformattingcollection/add/
---
## ConditionalFormattingCollection.Add method

Adds a FormatConditions to the collection.

```csharp
public int Add()
```

### Return Value

FormatConditions object index.

### Examples

```csharp
// Called: int index = worksheet.ConditionalFormattings.Add();
public static void Method_Add()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            // Add a conditional formatting collection to the worksheet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Define the cell area to apply the conditional formatting
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Add an above average condition to the collection
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Set the background color for the condition
            fc.Style.BackgroundColor = Color.Yellow;

            // Set properties for the above average condition
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells[&quot;A1&quot;].Value = 20;
            cells[&quot;A2&quot;].Value = 300;
            cells[&quot;A3&quot;].Value = 40;
            cells[&quot;A4&quot;].Value = 500;
            cells[&quot;A5&quot;].Value = 6;
            cells[&quot;A6&quot;].Value = 70;
            cells[&quot;A7&quot;].Value = 8;
            cells[&quot;A8&quot;].Value = 900;
            cells[&quot;A9&quot;].Value = 10;

            cells[&quot;C1&quot;].Value = 2;
            cells[&quot;C2&quot;].Value = 3;
            cells[&quot;C3&quot;].Value = 4;
            cells[&quot;C4&quot;].Value = 5;
            cells[&quot;C5&quot;].Value = 3;
            cells[&quot;C6&quot;].Value = 2;
            cells[&quot;C7&quot;].Value = 8;
            cells[&quot;C8&quot;].Value = 300;
            cells[&quot;C9&quot;].Value = 10;

            // Save the workbook
            workbook.Save(&quot;AboveAverageExample.xlsx&quot;);
            workbook.Save(&quot;AboveAverageExample.pdf&quot;);
        }
```

### See Also

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


