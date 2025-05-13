---
title: VbaProject.ValidatePassword
second_title: Aspose.Cells for .NET API Reference
description: VbaProject method. Validates protection password
type: docs
url: /net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Validates protection password.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | the password |

### Return Value

Whether password is the protection password of this VBA project

### Examples

```csharp
// Called: Assert.IsTrue(workbook.VbaProject.ValidatePassword("test"));
public void VbaProject_Method_ValidatePassword()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Assert.IsTrue(workbook.VbaProject.ValidatePassword("test"));
            
}
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


