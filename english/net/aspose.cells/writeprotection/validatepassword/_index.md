---
title: WriteProtection.ValidatePassword
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection method. Returns true if the specified password is the same as the writeprotection password the file was protected with
type: docs
url: /net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Returns true if the specified password is the same as the write-protection password the file was protected with.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The specified password. |

### Examples

```csharp
// Called: Assert.AreEqual(false, workbook.Settings.WriteProtection.ValidatePassword("12374"));
public void WriteProtection_Method_ValidatePassword()
{
    LoadOptions options = new LoadOptions(LoadFormat.Excel97To2003);
    options.Password = "1234";
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls",options);
    Assert.AreEqual(true, workbook.Settings.WriteProtection.ValidatePassword("1234"));
    Assert.AreEqual(false, workbook.Settings.WriteProtection.ValidatePassword("12374"));
}
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


