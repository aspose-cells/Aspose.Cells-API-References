---
title: FileFormatInfo.IsProtectedByRMS
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Gets whether the file is protected by Microsoft Rights Management Server
type: docs
url: /net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Gets whether the file is protected by Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "upload+simple+1.xls").IsProtectedByRMS);
public void FileFormatInfo_Property_IsProtectedByRMS()
{
    //Assert.IsTrue(CellsHelper.IsProtectedByRMS(Constants.sourcePath + "DRMExcel+document.xls"));
    //Assert.IsTrue(CellsHelper.IsProtectedByRMS(Constants.sourcePath + "DRMExcel+document.xlsx"));
    //Assert.IsFalse(CellsHelper.IsProtectedByRMS(Constants.sourcePath + "upload+simple+1.xls"));
    Assert.IsTrue(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "DRMExcel+document.xls").IsProtectedByRMS);
    Assert.IsTrue(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "DRMExcel+document.xlsx").IsProtectedByRMS);
    Assert.IsFalse(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "upload+simple+1.xls").IsProtectedByRMS);
}
```

### See Also

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


