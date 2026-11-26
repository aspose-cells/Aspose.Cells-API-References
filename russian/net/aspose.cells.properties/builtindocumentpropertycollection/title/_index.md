---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает заголовок документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Получает или задает заголовок документа.

```csharp
public string Title { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите свойство Title
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Отобразите свойство Title
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


