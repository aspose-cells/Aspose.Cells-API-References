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
public void AutoFitterOptions_Property_AutoFitWrappedTextType()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var worksheet = workbook.Worksheets["Sheet1"];

    var autoFitOpts = new AutoFitterOptions
    {
        IgnoreHidden = true,
        AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
    };

    worksheet.AutoFitColumns(autoFitOpts);
    worksheet.PageSetup.PrintArea = "DR_PUBv2_RANGE_1";
    workbook.Worksheets.ActiveSheetIndex = worksheet.Index;
    workbook.Save(Constants.destPath + "example.html");
    string text = File.ReadAllText(Constants.destPath + "example.html");
    Assert.IsTrue(text.IndexOf("##") == -1);
}
```

### See Also

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


