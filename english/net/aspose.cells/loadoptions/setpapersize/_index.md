---
title: LoadOptions.SetPaperSize
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions method. Sets the default print paper size from default printers setting
type: docs
url: /net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Sets the default print paper size from default printer's setting.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PaperSizeType | The default paper size. |

### Remarks

If there is no setting about paper size,MS Excel will use default printer's setting.

### Examples

```csharp
// Called: options.SetPaperSize(PaperSizeType.PaperA4);
[Test]
        public void Method_PaperSizeType_()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47034/&quot;;

            Aspose.Cells.HtmlLoadOptions options = new Aspose.Cells.HtmlLoadOptions(Aspose.Cells.LoadFormat.Html);

            options.AutoFitColsAndRows = true;
            options.AutoFitterOptions = new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
            };
            options.SetPaperSize(PaperSizeType.PaperA4);

            Workbook workbook = new Workbook(filePath + &quot;test.html&quot;, options);
            workbook.Save(CreateFolder(filePath) + @&quot;out.xls&quot;, Aspose.Cells.SaveFormat.Excel97To2003);
            ColumnCollection columns = workbook.Worksheets[0].Cells.Columns;
            //Assert.Greater(columns[0].Width, 19d);
            //Assert.Greater(columns[1].Width, 19d);
            //Assert.Greater(columns[2].Width, 19d);
            //Assert.Greater(columns[3].Width, 19d);
            //error, just pass
            Assert.Less(columns[0].Width, 12);
            Assert.Less(columns[1].Width, 12);
            Assert.Less(columns[2].Width, 12);
            Assert.Less(columns[3].Width, 12);

        }
```

### See Also

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


