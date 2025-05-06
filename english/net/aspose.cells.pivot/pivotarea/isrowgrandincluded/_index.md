---
title: PivotArea.IsRowGrandIncluded
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Indicates whether the row grand total is included
type: docs
url: /net/aspose.cells.pivot/pivotarea/isrowgrandincluded/
---
## PivotArea.IsRowGrandIncluded property

Indicates whether the row grand total is included.

```csharp
public bool IsRowGrandIncluded { get; set; }
```

### Examples

```csharp
// Called: pivotArea.IsRowGrandIncluded = true;
public static void Property_IsRowGrandIncluded()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Product&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Apples&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Oranges&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Bananas&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Sales&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(100);
            worksheet.Cells[&quot;B3&quot;].PutValue(150);
            worksheet.Cells[&quot;B4&quot;].PutValue(200);

            // Create a PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add(&quot;=A1:B4&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Add fields to the PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Create a PivotArea for the PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Output the PivotArea properties
            Console.WriteLine(&quot;Pivot Area Type: &quot; + pivotArea.RuleType);
            Console.WriteLine(&quot;Only Data: &quot; + pivotArea.OnlyData);
            Console.WriteLine(&quot;Is Row Grand Included: &quot; + pivotArea.IsRowGrandIncluded);

            // Save the workbook
            workbook.Save(&quot;PivotAreaTypeExample.xlsx&quot;);
        }
```

### See Also

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


