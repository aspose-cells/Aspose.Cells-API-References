---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает ключевые слова документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Получает или задает ключевые слова документа.

```csharp
public string Keywords { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить свойство Keywords
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Сохраните книгу
            workbook.Save("output_keywords.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить свойство Keywords
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Отобразить свойство Keywords
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


