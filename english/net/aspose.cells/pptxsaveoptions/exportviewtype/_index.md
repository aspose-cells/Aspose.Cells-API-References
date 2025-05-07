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
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET54781.xlsx");
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = Aspose.Cells.Slides.SlideViewType.View;
            //globalImageId = 1;
            workbook.Save(Constants.destPath + "CELLSNET54781.pptx", saveOptions);
            string slide1 = GetEntryText(Constants.destPath + "CELLSNET54781.pptx", @"ppt\slides\slide1.xml");
            Assert.IsTrue(slide1.IndexOf("<a:gridCol w=\"847725\">") != -1);
            Assert.IsTrue(slide1.IndexOf("a:lnR w=\"6350\"") != -1);
        }
```

### See Also

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


