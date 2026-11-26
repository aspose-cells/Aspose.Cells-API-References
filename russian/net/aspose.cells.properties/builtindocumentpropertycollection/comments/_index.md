---
title: "BuiltInDocumentPropertyCollection.Comments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает комментарии документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Получает или задает комментарии к документу.

```csharp
public string Comments { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Установите свойство Comments
            properties.Comments = "This is a sample comment for demonstration.";
            
            // Отобразите свойство Comments
            Console.WriteLine("Document Comments: " + properties.Comments);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


