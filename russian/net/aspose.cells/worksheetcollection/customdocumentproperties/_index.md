---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Возвращает коллекцию DocumentProperty, представляющую все пользовательские свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Возвращает коллекцию [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа электронной таблицы.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить пользовательские свойства документа
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Получить доступ и отобразить свойства
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### См. также

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


