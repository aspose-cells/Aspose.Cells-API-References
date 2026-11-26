---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает статус содержимого документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Получает или задает статус содержимого документа.

```csharp
public string ContentStatus { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить встроенные свойства документа, включая ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Сохраните книгу
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Отобразить свойство ContentStatus
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


