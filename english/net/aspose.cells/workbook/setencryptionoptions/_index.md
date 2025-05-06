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
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestStrongEncryption1.xls&quot;);
            workbook.Settings.Password = &quot;1234&quot;;
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            workbook.Save(Constants.destPath + &quot;TestStrongEncryption1.xls&quot;);
            //workbook.Open(Constants.destPath + &quot;TestStrongEncryption1.xls&quot;, FileFormatType.Excel2003, &quot;1234&quot;);
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = &quot;1234&quot;;
            workbook = new Workbook(Constants.destPath + &quot;TestStrongEncryption1.xls&quot;, loadOptions);

        }
```

### See Also

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


