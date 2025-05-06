---
title: AutoFitterOptions.AutoFitWrappedTextType
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the type of auto fitting wrapped text
type: docs
url: /net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Gets and sets the type of auto fitting wrapped text.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Examples

```csharp
// Called: AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
[Test]
        public void Property_AutoFitWrappedTextType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet52332.xlsx&quot;);
            var worksheet = workbook.Worksheets[&quot;Sheet1&quot;];

            var autoFitOpts = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            };

            worksheet.AutoFitColumns(autoFitOpts);
            worksheet.PageSetup.PrintArea = &quot;DR_PUBv2_RANGE_1&quot;;
            workbook.Worksheets.ActiveSheetIndex = worksheet.Index;
            workbook.Save(Constants.destPath + &quot;CellsNet52332.html&quot;);
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet52332.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;##&quot;) == -1);
        }
```

### See Also

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


