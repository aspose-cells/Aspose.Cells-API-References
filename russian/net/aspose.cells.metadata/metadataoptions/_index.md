---
title: "Класс MetadataOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Metadata.MetadataOptions. Представляет параметры загрузки метаданных файла"
type: docs
url: /ru/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Представляет параметры загрузки метаданных файла.

```csharp
public class MetadataOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Создаёт параметры загрузки метаданных. |

## Свойства

| Имя | Описание |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | Длина ключа. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Получает и задаёт тип загружаемых метаданных. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Представляет пароль шифрования файла Workbook. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsDemo
    {
        public static void MetadataOptionsExample()
        {
            // Создайте экземпляр MetadataOptions с определённым MetadataType
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Установить свойства
            options.Password = "your_password";
            options.KeyLength = 256;

            // Загрузите метаданные из существующей книги
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Добавьте пользовательское свойство документа
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Сохраните изменения метаданных в новый файл
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


