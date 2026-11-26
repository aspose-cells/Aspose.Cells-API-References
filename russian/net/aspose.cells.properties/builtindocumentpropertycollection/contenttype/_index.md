---
title: "BuiltInDocumentPropertyCollection.ContentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает тип содержимого документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

Получает или задает тип содержимого документа.

```csharp
public string ContentType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установите свойство ContentType
            workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";

            // Отобразите свойство ContentType
            Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);

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


