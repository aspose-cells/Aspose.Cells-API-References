---
title: "Workbook.SetEncryptionOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Установить параметры шифрования"
type: docs
url: /ru/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Установить параметры шифрования.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| encryptionType | EncryptionType | Тип шифрования. |
| keyLength | Int32 | Длина ключа. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить некоторые данные в лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Установить пароль и параметры шифрования
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Сохранить зашифрованный workbook
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Проверить, загрузив зашифрованный workbook
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### См. также

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


