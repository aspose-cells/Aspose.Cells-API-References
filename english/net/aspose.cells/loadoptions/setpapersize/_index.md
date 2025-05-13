---
title: LoadOptions.SetPaperSize
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions method. Sets the default print paper size from default printers setting
type: docs
url: /net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Sets the default print paper size from default printer's setting.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PaperSizeType | The default paper size. |

### Remarks

If there is no setting about paper size,MS Excel will use default printer's setting.

### Examples

```csharp
// Called: options.SetPaperSize(PaperSizeType.PaperA5);
public void LoadOptions_Method_SetPaperSize()
{
    LoadOptions options = new LoadOptions();
    options.SetPaperSize(PaperSizeType.PaperA5);
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls", options);
    Assert.AreEqual(PaperSizeType.PaperA5, workbook.Worksheets[0].PageSetup.PaperSize);
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Settings.PaperSize = PaperSizeType.PaperA5;
    Assert.AreEqual(PaperSizeType.PaperA5, workbook.Worksheets[0].PageSetup.PaperSize);
}
```

### See Also

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


