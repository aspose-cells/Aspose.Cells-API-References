---
title: Workbook.Unprotect
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Unprotects a workbook
type: docs
url: /net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Unprotects a workbook.

```csharp
public void Unprotect(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### Examples

```csharp
// Called: workbook.Unprotect("book"); // Correct password is "book"
public void Workbook_Method_Unprotect()
{
    LoadOptions lo = new LoadOptions() { Password = "excel" };
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx", lo);
    workbook.Unprotect("book"); // Correct password is "book"
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


