---
title: Workbook.UnprotectSharedWorkbook
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Unprotects a shared workbook
type: docs
url: /net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Unprotects a shared workbook.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### Examples

```csharp
// Called: wb.UnprotectSharedWorkbook("abcd");
public void Workbook_Method_UnprotectSharedWorkbook()
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


