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
public void DocxSaveOptions_Constructor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //workbook.Save(dir + "dest.pptx");
    DocxSaveOptions saveOptions = new DocxSaveOptions();
    saveOptions.SaveAsEditableShaps = true;
    workbook.Save(Constants.destPath + "example.docx", saveOptions);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.docx",
    "word/charts/chart1.xml", new string[] { "multiLvlStrRef" }, true));
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
// Called: w1.Save(destPathNetCore + "example.docx", new DocxSaveOptions(true));//for compare
public void DocxSaveOptions_Constructor()
{
    string path = PathNetCore + "TestDocx001/";
    Workbook w1 = new Workbook(path + "example.xlsx");
    w1.Save(destPathNetCore + "example.docx");
    w1.Save(destPathNetCore + "example.pdf");//for compare
    w1.Save(destPathNetCore + "example.docx", new DocxSaveOptions(true));//for compare

}
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


