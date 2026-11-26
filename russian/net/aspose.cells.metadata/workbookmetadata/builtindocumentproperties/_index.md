---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookMetadata. Возвращает коллекцию DocumentProperty, представляющую все встроенные свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Возвращает коллекцию [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/), представляющую все встроенные свойства документа электронной таблицы.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Сохранить книгу в файл
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Создать параметры метаданных для свойств документа
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Инициализировать метаданные рабочей книги
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Доступ к встроенным свойствам документа (только для чтения)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Отобразить некоторые встроенные свойства документа
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Изменить некоторые встроенные свойства (поскольку они доступны для чтения и записи)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Сохранить изменения метаданных
                metadata.Save(filePath);

                Console.WriteLine("\nBuilt-in properties have been updated and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


