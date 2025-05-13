---
title: Style.Font
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets a Font object
type: docs
url: /net/aspose.cells/style/font/
---
## Style.Font property

Gets a `Font` object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(b4.GetStyle().Font.IsBold, true);
public void Style_Property_Font()
{
    string filePath = Constants.PivotTableSourcePath + @"NET51735_";
    string savePath = CreateFolder(filePath);
    LoadOptions loadOptions = new LoadOptions(FileFormatUtil.DetectFileFormat(filePath + "Source.xlsm").LoadFormat);
    Workbook workbook = new Workbook(filePath + "Source.xlsm", loadOptions);

    PdfSaveOptions saveOptions = new PdfSaveOptions();
    workbook.Save(savePath + "out.pdf", saveOptions);

    Cells cells = workbook.Worksheets[0].Cells;
    Cell b4 = cells["B4"];
    Cell c4 = cells["C4"];
    Cell d4 = cells["D4"];
    Assert.AreEqual(b4.GetStyle().Font.IsBold, true);
    Assert.AreEqual(c4.GetStyle().Font.IsBold, false);
    Assert.AreEqual(d4.GetStyle().Font.IsBold, true);

    Assert.AreEqual(b4.GetStyle().ForegroundColor, Color.Empty);
}
```

### See Also

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


