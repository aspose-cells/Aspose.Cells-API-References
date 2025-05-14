---
title: TxtLoadOptions.SeparatorString
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets a string value as separator
type: docs
url: /net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Gets and sets a string value as separator.

```csharp
public string SeparatorString { get; set; }
```

### Examples

```csharp
// Called: loadOptions.SeparatorString = "&^";
public void TxtLoadOptions_Property_SeparatorString()
{
    string FileName = Constants.sourcePath + "TestWorkbook\\Book1.xls";
    Workbook workbook = new Workbook(FileName);
    TxtSaveOptions saveOptions = new TxtSaveOptions();
    saveOptions.TrimLeadingBlankRowAndColumn = false;
    saveOptions.SeparatorString = "&^";
    workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

    TxtLoadOptions loadOptions = new TxtLoadOptions();
    loadOptions.SeparatorString = "&^";
    workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


