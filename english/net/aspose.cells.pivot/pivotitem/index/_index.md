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
private void PivotItem_Property_Index(string file, string filePath)
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

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


