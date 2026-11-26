---
title: "WorkbookMetadata.Options"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookMetadata. Получает параметры метаданных"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Получает параметры метаданных.

```csharp
public MetadataOptions Options { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyOptionsDemo
    {
        public static void Run()
        {
            // Создать параметры метаданных для свойств документа
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Создать новый экземпляр метаданных книги с параметрами
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Отобразить текущие значения параметров
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Получить доступ к встроенным свойствам документа
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Добавить пользовательские свойства документа
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Сохранить изменения метаданных
            metadata.Save("output.xlsx");

            // Создать новые параметры для шифрования
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### См. также

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


