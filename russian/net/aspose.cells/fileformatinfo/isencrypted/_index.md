---
title: "FileFormatInfo.IsEncrypted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFormatInfo. Возвращает true, если документ зашифрован и требует пароль для открытия"
type: docs
url: /ru/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Возвращает true, если документ зашифрован и требует пароль для открытия.

```csharp
public bool IsEncrypted { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Обнаружить формат файла без шифрования
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Обнаружить формат зашифрованного файла
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Загрузить зашифрованный файл с паролем
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### См. также

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


