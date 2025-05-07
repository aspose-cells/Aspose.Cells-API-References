---
title: HtmlSaveOptions.HtmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions constructor. Creates options for saving html file
type: docs
url: /net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Creates options for saving html file.

```csharp
public HtmlSaveOptions()
```

### Examples

```csharp
// Called: HtmlSaveOptions saveOptions = new HtmlSaveOptions();
private void HtmlSaveOptions_Constructor(int count, bool f)
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49413.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.IgnoreInvisibleShapes = f;
            workbook.Save(_destFilesPath + "CELLSNET49413.html", saveOptions);
            workbook = new Workbook(_destFilesPath + "CELLSNET49413.html");
            Assert.AreEqual(count, workbook.Worksheets[0].Shapes.Count);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving htm file.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Html or MHtml, otherwise the saved format will be set as Html automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


