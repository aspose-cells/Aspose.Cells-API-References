---
title: HtmlSaveOptions.IgnoreInvisibleShapes
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicate whether exporting those not visible shapes
type: docs
url: /net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Indicate whether exporting those not visible shapes

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Remarks

The default values is false.

### Examples

```csharp
// Called: saveOptions.IgnoreInvisibleShapes = f;
private void HtmlSaveOptions_Property_IgnoreInvisibleShapes(int count, bool f)
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.IgnoreInvisibleShapes = f;
            workbook.Save(_destFilesPath + "example.html", saveOptions);
            workbook = new Workbook(_destFilesPath + "example.html");
            Assert.AreEqual(count, workbook.Worksheets[0].Shapes.Count);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


