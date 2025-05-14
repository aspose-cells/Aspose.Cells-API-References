---
title: LoadOptions.DefaultStyleSettings
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets the default style settings for initializing styles of the workbook
type: docs
url: /net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Gets the default style settings for initializing styles of the workbook

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Examples

```csharp
// Called: loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
public void LoadOptions_Property_DefaultStyleSettings()
{
    string filePath = Constants.PivotTableSourcePath + @"NET51595_";
    string savePath = CreateFolder(filePath);

    LoadOptions loadOptions = new LoadOptions(FileFormatUtil.DetectFileFormat(filePath + "book.xlsm").LoadFormat);
    loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
    Workbook workbook = new Workbook(filePath + "book.xlsm", loadOptions);

    PdfSaveOptions saveOptions = new PdfSaveOptions();
    workbook.Save(savePath + "out.pdf", saveOptions);

    Cell o10 = workbook.Worksheets[0].Cells["O10"];
    Assert.AreEqual(o10.GetStyle().VerticalAlignment, TextAlignmentType.Center);

    Cell a7 = workbook.Worksheets[0].Cells["A7"];
    Assert.AreEqual(a7.GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
}
```

### See Also

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


