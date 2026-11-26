---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает имя автора документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Получает или задает имя автора документа.

```csharp
public string Author { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить свойство автора
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Отобразить свойство автора
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


