---
title: PivotTable.ShowDrill
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets whether showing expand/collapse buttons
type: docs
url: /net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Gets and sets whether showing expand/collapse buttons.

```csharp
public bool ShowDrill { get; set; }
```

### Examples

```csharp
// Called: pt.ShowDrill = true;
private void PivotTable_Property_ShowDrill(string file, string filePath)
        {
            var book = new Workbook(filePath + file);
            string sheetName = "Pivot";
            var sheet = book.Worksheets[sheetName];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                Console.WriteLine("Refreshing Pivot table {pt.Name} in {sheet.Name}");
                pt.RefreshData();
                pt.CalculateData();
                pt.PreserveFormatting = true;
                pt.EnableDrilldown = true;
                pt.ShowDrill = true;
            }

            Assert.AreEqual(book.Worksheets["Pivot"].Cells["A93"].StringValue, "FX_Carry_Value");

            book.Save(CreateFolder(filePath) + @"out_Bug_SourceData_AfterRefresh.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


