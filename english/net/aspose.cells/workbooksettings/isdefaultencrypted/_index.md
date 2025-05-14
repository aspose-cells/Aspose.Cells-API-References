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
// Called: Assert.IsFalse(workbook.Settings.IsDefaultEncrypted);
public void WorkbookSettings_Property_IsDefaultEncrypted()
{
    Workbook workbook = new Workbook(FileFormatType.Xlsx);
    Assert.IsFalse(workbook.Settings.IsDefaultEncrypted);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


