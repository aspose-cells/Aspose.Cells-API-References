---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает категорию документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Получает или задает категорию документа.

```csharp
public string Category { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            var workbook = new Workbook();
            
            // Установить встроенные свойства документа
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // Сохранить в поток памяти
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // Загрузите книгу обратно из потока
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // Отобразите свойства
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


