---
title: WriteProtection.IsWriteProtected
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Indicates whether this workbook is write protected
type: docs
url: /net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Indicates whether this workbook is write protected.

```csharp
public bool IsWriteProtected { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
public void WriteProtection_Property_IsWriteProtected()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsb");
    Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
    Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword("5678"));
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
    Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword("5678")); 
}
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


