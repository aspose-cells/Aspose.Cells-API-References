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
[Test]
        public void Property_IsWriteProtected()
        {
            Workbook workbook = new Workbook();
            Assert.IsFalse(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Settings.WriteProtection.Password = "test";
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + "WriteProtect01.xlsx");
            workbook = new Workbook(Constants.destPath + "WriteProtect01.xlsx");
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + "WriteProtect01.xls");
            workbook = new Workbook(Constants.destPath + "WriteProtect01.xls");
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + "WriteProtect01.xlsb");
            workbook = new Workbook(Constants.destPath + "WriteProtect01.xlsb");
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


