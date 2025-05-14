---
title: FileFormatInfo.IsEncrypted
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Returns true if the document is encrypted and requires a password to open
type: docs
url: /net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Returns true if the document is encrypted and requires a password to open.

```csharp
public bool IsEncrypted { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(fileInfo.IsEncrypted);
public void FileFormatInfo_Property_IsEncrypted()
{
    FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(Constants.sourcePath + "example.xlsx");
    Assert.IsFalse(fileInfo.IsEncrypted);
    Aspose.Cells.LoadOptions cellsLoadOptionsWithPassword = new Aspose.Cells.LoadOptions(Aspose.Cells.LoadFormat.Auto);
    cellsLoadOptionsWithPassword.Password = "password";
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx", cellsLoadOptionsWithPassword);
    cellsLoadOptionsWithPassword = new Aspose.Cells.LoadOptions(Aspose.Cells.LoadFormat.Auto);
    cellsLoadOptionsWithPassword.Password = "password";
    workbook = new Workbook(Constants.sourcePath + "example.xls", cellsLoadOptionsWithPassword);
}
```

### See Also

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


