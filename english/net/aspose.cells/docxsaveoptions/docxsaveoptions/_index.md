---
title: DocxSaveOptions.DocxSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: DocxSaveOptions constructor. Represents options of saving .docx file
type: docs
url: /net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Represents options of saving .docx file.

```csharp
public DocxSaveOptions()
```

### Examples

```csharp
// Called: DocxSaveOptions saveOptions = new DocxSaveOptions();
[Test]
        public void DocxSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET58083.xlsx&quot;);
            //workbook.Save(dir + &quot;dest.pptx&quot;);
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            workbook.Save(Constants.destPath + &quot;CELLSNET58083.docx&quot;, saveOptions);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET58083.docx&quot;,
            &quot;word/charts/chart1.xml&quot;, new string[] { &quot;m/d/yyyy&quot; }, true));
        }
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Represents options of saving .docx file.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | If True, the workbook will be converted into some pictures of .docx file. If False, the workbook will be converted into some tables of .docx file. |

### Examples

```csharp
// Called: w1.Save(destPathNetCore + &amp;quot;TestDocx001_image.docx&amp;quot;, new DocxSaveOptions(true));//for compare
[Test]
        public void DocxSaveOptions_Constructor()
        {
            string path = PathNetCore + &quot;TestDocx001/&quot;;
            Workbook w1 = new Workbook(path + &quot;TestDocx001.xlsx&quot;);
            w1.Save(destPathNetCore + &quot;TestDocx001.docx&quot;);
            w1.Save(destPathNetCore + &quot;TestDocx001.pdf&quot;);//for compare
            w1.Save(destPathNetCore + &quot;TestDocx001_image.docx&quot;, new DocxSaveOptions(true));//for compare

        }
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


