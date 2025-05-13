---
title: DocxSaveOptions.SaveAsEditableShaps
second_title: Aspose.Cells for .NET API Reference
description: DocxSaveOptions property. Save all drawing objecgts as editable shapes in word file.So you can edit them in Word
type: docs
url: /net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Save all drawing objecgts as editable shapes in word file.So you can edit them in Word.

```csharp
public bool SaveAsEditableShaps { get; set; }
```

### Examples

```csharp
// Called: saveOptions.SaveAsEditableShaps = true;
public void DocxSaveOptions_Property_SaveAsEditableShaps()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //workbook.Save(dir + "dest.pptx");
    DocxSaveOptions saveOptions = new DocxSaveOptions();
    saveOptions.SaveAsEditableShaps = true;
    workbook.Save(Constants.destPath + "example.docx", saveOptions);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.docx",
    "word/document.xml", new string[] { "http://schemas.microsoft.com/office/drawing/2014/chartex" }, true));
}
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


