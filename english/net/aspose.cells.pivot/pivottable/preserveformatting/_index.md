---
title: PivotTable.PreserveFormatting
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated
type: docs
url: /net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

```csharp
public bool PreserveFormatting { get; set; }
```

### Examples

```csharp
// Called: pt.PreserveFormatting = true;
private void Property_PreserveFormatting(string file, string filePath)
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

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


