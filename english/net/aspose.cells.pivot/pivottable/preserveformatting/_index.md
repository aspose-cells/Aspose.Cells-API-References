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
private void PivotTable_Property_PreserveFormatting(string file, string filePath)
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

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


