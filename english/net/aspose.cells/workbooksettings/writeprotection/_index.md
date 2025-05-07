---
title: WorkbookSettings.WriteProtection
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Provides access to the workbook write protection options
type: docs
url: /net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Provides access to the workbook write protection options.

```csharp
public WriteProtection WriteProtection { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword("5678"));
[Test]
        public void Property_WriteProtection()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet43261.xlsb");
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword("5678"));
            workbook.Save(Constants.destPath + "CellsNet43261.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet43261.xlsb");
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword("5678")); 
        }
```

### See Also

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


