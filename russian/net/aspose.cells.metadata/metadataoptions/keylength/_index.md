---
title: "MetadataOptions.KeyLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MetadataOptions. Длина ключа"
type: docs
url: /ru/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

Длина ключа.

```csharp
public int KeyLength { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Создать параметры метаданных с типом свойств документа
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Установить свойства шифрования, включая KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Создать метаданные для новой рабочей книги
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Добавить пользовательское свойство
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Сохранить с шифрованием
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### См. также

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


