---
title: PivotField.HideItemDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specific PivotItem in a pivot field is hidden detail
type: docs
url: /net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Sets whether the specific PivotItem in a pivot field is hidden detail.

```csharp
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHiddenDetail | Boolean | whether the specific PivotItem is hidden |

### Examples

```csharp
// Called: pf.HideItemDetail(pi.Index, true);
private void Method_Boolean_(string file, string filePath)
        {
            var book = new Workbook(filePath + file);
            string sheetName = "Pivot";
            var sheet = book.Worksheets[sheetName];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                Console.WriteLine("Refreshing Pivot table {pt.Name} in {sheet.Name}");
                pt.RefreshData();

                PivotField pf = pt.RowFields["Bucket"];
                //Should Hide the item detail for Rates_Carry_Value.
                PivotItem pi = pf.PivotItems["Rates_Carry_Value"];
                pf.HideItemDetail(pi.Index, true);

                pt.CalculateData();
                pt.PreserveFormatting = true;
                pt.EnableDrilldown = true;
                pt.ShowDrill = true;
            }

            Assert.AreEqual(book.Worksheets["Pivot"].Cells["A85"].StringValue, "Rates_Carry_Value");

            book.Save(CreateFolder(filePath) + @"out_Bug_SourceData_PivotExpanded_AfterRefresh.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


