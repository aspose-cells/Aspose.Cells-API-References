---
title: PivotTable.EnableDrilldown
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets whether drilldown is enabled
type: docs
url: /net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Gets whether drilldown is enabled.

```csharp
public bool EnableDrilldown { get; set; }
```

### Examples

```csharp
// Called: pt.EnableDrilldown = true;
private void Property_EnableDrilldown(string file, string filePath)
        {
            var book = new Workbook(filePath + file);
            string sheetName = &quot;Pivot&quot;;
            var sheet = book.Worksheets[sheetName];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                Console.WriteLine(&quot;Refreshing Pivot table {pt.Name} in {sheet.Name}&quot;);
                pt.RefreshData();
                pt.CalculateData();
                pt.PreserveFormatting = true;
                pt.EnableDrilldown = true;
                pt.ShowDrill = true;
            }

            Assert.AreEqual(book.Worksheets[&quot;Pivot&quot;].Cells[&quot;A93&quot;].StringValue, &quot;FX_Carry_Value&quot;);

            book.Save(CreateFolder(filePath) + @&quot;out_Bug_SourceData_AfterRefresh.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


