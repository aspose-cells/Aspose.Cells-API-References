---
title: Workbook.ProtectSharedWorkbook
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Protects a shared workbook
type: docs
url: /net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Protects a shared workbook.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to protect the workbook. |

### Examples

```csharp
// Called: wb.ProtectSharedWorkbook("abcd");
public void Workbook_Method_ProtectSharedWorkbook()
{
    Workbook wb = new Workbook();
    wb.ProtectSharedWorkbook("abcd");
    wb.Save(Constants.destPath + "ProectSharedWorkbook.xlsx");
    wb = new Aspose.Cells.Workbook(Constants.destPath + "ProectSharedWorkbook.xlsx");
    Assert.IsTrue(wb.Settings.IsProtected);
    wb.UnprotectSharedWorkbook("abcd");
    wb.Save(Constants.destPath + "UnProectSharedWorkbook.xlsx");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


