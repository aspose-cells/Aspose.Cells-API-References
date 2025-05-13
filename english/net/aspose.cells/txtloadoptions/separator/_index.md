---
title: TxtLoadOptions.Separator
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets character separator of text file
type: docs
url: /net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Gets and sets character separator of text file.

```csharp
public char Separator { get; set; }
```

### Examples

```csharp
// Called: loadOptions.Separator = '*';
public void TxtLoadOptions_Property_Separator()
{
    string FileName = Constants.sourcePath + "TestWorkbook\\Book1.xls";
    Workbook workbook = new Workbook(FileName);
    TxtSaveOptions saveOptions = new TxtSaveOptions();
    saveOptions.Separator = '*';
    workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

    TxtLoadOptions loadOptions = new TxtLoadOptions();
    loadOptions.Separator = '*';
    workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


