---
title: SaveOptions.CachedFileFolder
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. The cached file folder is used to store some large data
type: docs
url: /net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

The cached file folder is used to store some large data.

```csharp
public string CachedFileFolder { get; set; }
```

### Examples

```csharp
// Called: saveOptions.CachedFileFolder = Constants.destPath;
public void SaveOptions_Property_CachedFileFolder()
{
    string file = Constants.bugFilePath + "RollRate.xls";
    Workbook workbook = new Workbook(file);
    SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions(SaveFormat.SpreadsheetML);
    saveOptions.CachedFileFolder = Constants.destPath;
    workbook.Save(Constants.destPath + "testSave.xml", saveOptions);
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


