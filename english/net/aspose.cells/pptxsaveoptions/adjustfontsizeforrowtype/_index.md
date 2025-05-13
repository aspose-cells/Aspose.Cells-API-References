---
title: PptxSaveOptions.AdjustFontSizeForRowType
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions property. Represents what type of line needs to be adjusted size of font if height of row is small
type: docs
url: /net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Represents what type of line needs to be adjusted size of font if height of row is small.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.AdjustFontSizeForRowType = Aspose.Cells.Slides.AdjustFontSizeForRowType.EmptyRows;
public void PptxSaveOptions_Property_AdjustFontSizeForRowType()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
          
    PptxSaveOptions saveOptions = new PptxSaveOptions();
    saveOptions.IgnoreHiddenRows = true;
    saveOptions.AdjustFontSizeForRowType = Aspose.Cells.Slides.AdjustFontSizeForRowType.EmptyRows;
    wb.Save(Constants.destPath + "example.pptx", saveOptions);
    string slide1 = GetEntryText(Constants.destPath + "example.pptx", @"ppt\slides\slide1.xml");
    Assert.IsTrue(slide1.IndexOf("sz=\"100\"") != -1);
}
```

### See Also

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


