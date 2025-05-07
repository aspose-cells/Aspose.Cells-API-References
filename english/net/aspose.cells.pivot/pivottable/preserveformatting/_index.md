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
// Called: pivottable.PreserveFormatting = true;
[Test]
        public void Property_PreserveFormatting()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46882_";
            Workbook wb = new Workbook(filePath + "SampleFile.xlsx");
            Worksheet ws = wb.Worksheets[0];
            ws.PageSetup.PrintArea = "";
            PivotTable pivottable = ws.PivotTables[0];
            pivottable.RefreshData();

            pivottable.PreserveFormatting = true;
            wb.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            pivottable.RefreshData();
            pivottable.CalculateRange();
            pivottable.CalculateData();

            Cells cells = ws.Cells;
            Assert.AreEqual(cells["A2"].StringValue, "Sep");
            Assert.AreEqual(cells["A26"].StringValue, "Aug");
            Assert.AreEqual(cells["B1"].GetStyle().ForegroundColor, Color.FromArgb(255, 0, 176, 80));

            wb.Save(CreateFolder(filePath) + "out.pdf", Aspose.Cells.SaveFormat.Pdf);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


