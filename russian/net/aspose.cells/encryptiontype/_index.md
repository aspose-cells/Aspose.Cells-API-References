---
title: "Перечисление EncryptionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.EncryptionType. Тип шифрования. Используется только в excel2003. Мы будем шифровать книгу 2007/2010 с использованием SHA AES так же, как делает Excel, и это EncryptionType будет игнорироваться."
type: docs
url: /ru/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Тип шифрования. Используется только в excel2003. Мы будем шифровать рабочие книги 2007/2010 с помощью SHA AES так же, как делает Excel, и этот EncryptionType будет игнорироваться.

```csharp
public enum EncryptionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| XOR | `0` | Алгоритм шифрования XOR. |
| Compatible | `1` | Совместим с Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Улучшенное шифрование. |
| StrongCryptographicProvider | `3` | Сильный алгоритм шифрования. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить параметры шифрования для книги
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Применить настройки шифрования
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Защитить книгу паролем
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Сохраните книгу
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


