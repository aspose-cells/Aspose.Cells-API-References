---
title: PptxSaveOptions.IgnoreHiddenRows
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions property. Inidicates whether ignoring hidden rows when converting Excel to PowerPoint
type: docs
url: /net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Inidicates whether ignoring hidden rows when converting Excel to PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Examples

```csharp
// Called: saveOptions.IgnoreHiddenRows = true;
public void PptxSaveOptions_Property_IgnoreHiddenRows()
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


