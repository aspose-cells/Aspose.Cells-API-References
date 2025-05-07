---
title: WorkbookSettings.IsDefaultEncrypted
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked
type: docs
url: /net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Remarks

The default value is false now. It's same as MS Excel 2013.

### Examples

```csharp
// Called: workbook.Settings.IsDefaultEncrypted = false;
[Test]
        public void Property_IsDefaultEncrypted()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.IsDefaultEncrypted = false;
            workbook.Protect(ProtectionType.All, "1234");
            MemoryStream ms = Util.SaveAsBuffer(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(ms.ReadByte(), 0x50);
            Assert.AreEqual(ms.ReadByte(), 0x4b);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


