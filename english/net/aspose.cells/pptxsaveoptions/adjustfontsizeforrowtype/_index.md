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
[Test]
        public void Property_AdjustFontSizeForRowType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET54742.xlsx&quot;);
          
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            saveOptions.AdjustFontSizeForRowType = Aspose.Cells.Slides.AdjustFontSizeForRowType.EmptyRows;
            wb.Save(Constants.destPath + &quot;CELLSNET54742.pptx&quot;, saveOptions);
            string slide1 = GetEntryText(Constants.destPath + &quot;CELLSNET54742.pptx&quot;, @&quot;ppt\slides\slide1.xml&quot;);
            Assert.IsTrue(slide1.IndexOf(&quot;sz=\&quot;100\&quot;&quot;) != -1);
        }
```

### See Also

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


