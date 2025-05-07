---
title: AutoFitterOptions.IgnoreHidden
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Ignores the hidden rows/columns
type: docs
url: /net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignores the hidden rows/columns.

```csharp
public bool IgnoreHidden { get; set; }
```

### Examples

```csharp
// Called: IgnoreHidden = true,
[Test]
        public void Property_IgnoreHidden()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52332.xlsx");
            var worksheet = workbook.Worksheets["Sheet1"];

            var autoFitOpts = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            };

            worksheet.AutoFitColumns(autoFitOpts);
            worksheet.PageSetup.PrintArea = "DR_PUBv2_RANGE_1";
            workbook.Worksheets.ActiveSheetIndex = worksheet.Index;
            workbook.Save(Constants.destPath + "CellsNet52332.html");
            string text = File.ReadAllText(Constants.destPath + "CellsNet52332.html");
            Assert.IsTrue(text.IndexOf("##") == -1);
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


