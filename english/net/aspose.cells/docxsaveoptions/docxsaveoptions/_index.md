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
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET58083.xlsx");
            //workbook.Save(dir + "dest.pptx");
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            workbook.Save(Constants.destPath + "CELLSNET58083.docx", saveOptions);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CELLSNET58083.docx",
            "word/charts/chart1.xml", new string[] { "m/d/yyyy" }, true));
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
// Called: w1.Save(destPathNetCore + "TestDocx001_image.docx", new DocxSaveOptions(true));//for compare
[Test]
        public void DocxSaveOptions_Constructor()
        {
            string path = PathNetCore + "TestDocx001/";
            Workbook w1 = new Workbook(path + "TestDocx001.xlsx");
            w1.Save(destPathNetCore + "TestDocx001.docx");
            w1.Save(destPathNetCore + "TestDocx001.pdf");//for compare
            w1.Save(destPathNetCore + "TestDocx001_image.docx", new DocxSaveOptions(true));//for compare

        }
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


