---
title: SaveOptions.CreateDirectory
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. If true and the directory does not exist the directory will be automatically created before saving the file
type: docs
url: /net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

If true and the directory does not exist, the directory will be automatically created before saving the file.

```csharp
public bool CreateDirectory { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: saveOptions.CreateDirectory = true;
public void SaveOptions_Property_CreateDirectory()
{
    Workbook workbook = new Workbook();
    XlsSaveOptions saveOptions = new XlsSaveOptions();
    saveOptions.CreateDirectory = true;
    workbook.Save(Constants.destPath + @"example.xls",saveOptions);
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


