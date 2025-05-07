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
// Called: workbook.SetEncryptionOptions(EncryptionType.Compatible, 512);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Password = "test";
            workbook.SetEncryptionOptions(EncryptionType.Compatible, 512);
            workbook.Save(Constants.destPath + "CELLSNET46118.xls");

            LoadOptions options = new LoadOptions();
            options.Password = "test";
            workbook = new Workbook(Constants.destPath + "CELLSNET46118.xls", options);
        }
```

### See Also

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


