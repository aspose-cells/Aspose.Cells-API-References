---
title: Workbook.SetEncryptionOptions
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Set Encryption Options
type: docs
url: /net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Set Encryption Options.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | EncryptionType | The encryption type. |
| keyLength | Int32 | The key length. |

### Examples

```csharp
// Called: workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
public void Workbook_Method_SetEncryptionOptions()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestStrongEncryption1.xls");
    workbook.Settings.Password = "1234";
    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
    workbook.Save(Constants.destPath + "TestStrongEncryption1.xls");
    //workbook.Open(Constants.destPath + "TestStrongEncryption1.xls", FileFormatType.Excel2003, "1234");
    LoadOptions loadOptions = new LoadOptions();
    loadOptions.Password = "1234";
    workbook = new Workbook(Constants.destPath + "TestStrongEncryption1.xls", loadOptions);

}
```

### See Also

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


