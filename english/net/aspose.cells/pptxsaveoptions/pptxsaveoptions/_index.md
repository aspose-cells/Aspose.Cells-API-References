---
title: PptxSaveOptions.PptxSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions constructor. Represents the pptx save options
type: docs
url: /net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Represents the pptx save options.

```csharp
public PptxSaveOptions()
```

### Examples

```csharp
// Called: PptxSaveOptions saveOptions = new PptxSaveOptions();
[Test]
        public void PptxSaveOptions_Constructor()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET54753.xlsx");
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            wb.Save(Constants.destPath + "CELLSNET54753.pptx", saveOptions);
            string slide1 = GetEntryText(Constants.destPath + "CELLSNET54753.pptx", @"ppt\slides\slide1.xml");
            Assert.IsTrue(slide1.IndexOf("Qtr1") == -1);
        }
```

### See Also

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Represents options of saving .pptx file.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | If True, the workbook will be converted into some pictures of .pptx file. If False, the workbook will be converted into some tables of .pptx file. |

### See Also

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


