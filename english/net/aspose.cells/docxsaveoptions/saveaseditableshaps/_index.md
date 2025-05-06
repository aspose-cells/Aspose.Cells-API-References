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
[Test]
        public void Property_SaveAsEditableShaps()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET58082.xlsx&quot;);
            //workbook.Save(dir + &quot;dest.pptx&quot;);
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            workbook.Save(Constants.destPath + &quot;CELLSNET58082.docx&quot;, saveOptions);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET58082.docx&quot;,
            &quot;word/charts/chart1.xml&quot;, new string[] { &quot;multiLvlStrRef&quot; }, true));
        }
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


