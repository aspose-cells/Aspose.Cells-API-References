---
title: "MetadataOptions.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MetadataOptions. Представляет пароль шифрования файла Workbook"
type: docs
url: /ru/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Представляет пароль шифрования файла Workbook.

```csharp
public string Password { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать параметры метаданных с защитой паролем
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Создать новую рабочую книгу и сначала сохранить её
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Загрузить метаданные из сохранённого файла
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Добавить пользовательское свойство документа
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Сохранить с метаданными
            metadata.Save(filePath);
        }
    }
}
```

### См. также

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


