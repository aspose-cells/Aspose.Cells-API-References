---
title: StyleFlag.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Horizontal alignment setting will be applied
type: docs
url: /net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Horizontal alignment setting will be applied.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: flag.HorizontalAlignment = true;
[Test]
        public void Property_HorizontalAlignment()
        {
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Port.\r\nBeginning\r\nMarket Value");
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Right;
            flag.WrapText = true;
            flag.HorizontalAlignment = true;
            var range = worksheet.Cells.CreateRange("A1:A1");
            range.ApplyStyle(style, flag);
            cell.Characters(0, cell.StringValue.Length - 3).Font.IsBold = true;
            var columnOptions = new AutoFitterOptions { AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph };
            worksheet.AutoFitColumns(columnOptions);
            var options = new AutoFitterOptions { AutoFitMergedCells = true };
            worksheet.AutoFitRows(options);
           Assert.AreEqual(90,worksheet.Cells.GetColumnWidthPixel(0));
            workbook.Save(Constants.destPath + "CellsNet47016.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


