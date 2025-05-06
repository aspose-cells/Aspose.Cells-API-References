---
title: CellArea.CompareTo
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Compare two CellArea objects according to their topleft corner
type: docs
url: /net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Compare two CellArea objects according to their top-left corner.

```csharp
public int CompareTo(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Return Value

If two corners are in different rows, then compare their row index. Otherwise compare their column index. If two corners are same, then 0 will be returned.

### Examples

```csharp
// Called: int comparisonResult = ca.CompareTo(ca2);
public static void Method_Object_()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[&quot;B2&quot;].PutValue(4);
            worksheet.Cells[&quot;B5&quot;].PutValue(20);
            worksheet.Cells[&quot;B8&quot;].PutValue(50);
            worksheet.Cells[&quot;C2&quot;].PutValue(8);
            worksheet.Cells[&quot;C7&quot;].PutValue(15);
            worksheet.Cells[&quot;C9&quot;].PutValue(30);

            // Create Cell Area
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Add a conditional formatting rule to the worksheet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &quot;5&quot;, &quot;30&quot;);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Save the workbook
            workbook.Save(&quot;CellAreaExample.xlsx&quot;);
            workbook.Save(&quot;CellAreaExample.pdf&quot;);

            // Demonstrate the ToString method
            Console.WriteLine(ca.ToString());

            // Demonstrate the CompareTo method
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($&quot;Comparison result: {comparisonResult}&quot;);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


