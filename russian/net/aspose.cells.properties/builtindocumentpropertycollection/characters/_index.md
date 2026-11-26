---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Представляет оценку количества символов в документе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

Представляет оценку количества символов в документе.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Отобразите текущее значение Characters (устаревшее свойство)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // Установите новое значение для Characters (устаревшее свойство)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // Добавьте некоторое содержимое, чтобы продемонстрировать эффект свойства
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // Сохраните книгу
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


