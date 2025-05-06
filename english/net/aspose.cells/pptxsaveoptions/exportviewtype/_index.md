---
title: PptxSaveOptions.ExportViewType
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions property. Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing
type: docs
url: /net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportViewType = Aspose.Cells.Slides.SlideViewType.View;
[Test]
        public void Property_ExportViewType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET54781.xlsx&quot;);
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = Aspose.Cells.Slides.SlideViewType.View;
            //globalImageId = 1;
            workbook.Save(Constants.destPath + &quot;CELLSNET54781.pptx&quot;, saveOptions);
            string slide1 = GetEntryText(Constants.destPath + &quot;CELLSNET54781.pptx&quot;, @&quot;ppt\slides\slide1.xml&quot;);
            Assert.IsTrue(slide1.IndexOf(&quot;&lt;a:gridCol w=\&quot;847725\&quot;&gt;&quot;) != -1);
            Assert.IsTrue(slide1.IndexOf(&quot;a:lnR w=\&quot;6350\&quot;&quot;) != -1);
        }
```

### See Also

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


