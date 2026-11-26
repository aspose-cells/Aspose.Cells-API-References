---
title: "Перечисление MetadataType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Metadata.MetadataType. Представляет тип метаданных"
type: docs
url: /ru/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Представляет тип метаданных.

```csharp
[Flags]
public enum MetadataType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Encryption | `1` | Шифрует файл. |
| Decryption | `2` | Расшифровывает файл. |
| DocumentProperties | `4` | Загружает свойства файла. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class MetadataTypeDemo
    {
        public static void MetadataTypeExample()
        {
            // Определить путь к файлу
            string filePath = "MetadataTypeExample_original.xlsx";

            // Создать MetadataOptions для DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Загрузить метаданные рабочей книги
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Получить доступ к пользовательским свойствам документа
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Отобразить некоторые встроенные свойства
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Добавить пользовательское свойство
            customProperties.Add("MyCustomProperty", "CustomValue");

            // сохранить в другой файл
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


