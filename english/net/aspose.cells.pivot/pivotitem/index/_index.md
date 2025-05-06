---
title: PivotItem.Index
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets the index of the pivot item in cache field
type: docs
url: /net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Gets the index of the pivot item in cache field.

```csharp
public int Index { get; set; }
```

### Examples

```csharp
// Called: pf.HideItemDetail(pi.Index, true);
private void Property_Index(string file, string filePath)
        {
            var book = new Workbook(filePath + file);
            string sheetName = &quot;Pivot&quot;;
            var sheet = book.Worksheets[sheetName];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                Console.WriteLine(&quot;Refreshing Pivot table {pt.Name} in {sheet.Name}&quot;);
                pt.RefreshData();

                PivotField pf = pt.RowFields[&quot;Bucket&quot;];
                //Should Hide the item detail for Rates_Carry_Value.
                PivotItem pi = pf.PivotItems[&quot;Rates_Carry_Value&quot;];
                pf.HideItemDetail(pi.Index, true);

                pt.CalculateData();
                pt.PreserveFormatting = true;
                pt.EnableDrilldown = true;
                pt.ShowDrill = true;
            }

            Assert.AreEqual(book.Worksheets[&quot;Pivot&quot;].Cells[&quot;A85&quot;].StringValue, &quot;Rates_Carry_Value&quot;);

            book.Save(CreateFolder(filePath) + @&quot;out_Bug_SourceData_PivotExpanded_AfterRefresh.xlsx&quot;);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


