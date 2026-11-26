---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Указывает, актуальны ли гиперссылки в документе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Указывает, актуальны ли гиперссылки в документе.

```csharp
public bool LinksUpToDate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к встроенной коллекции свойств документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установите свойство LinksUpToDate, чтобы указать, являются ли гиперссылки текущими
            builtInProperties.LinksUpToDate = true;

            // Добавьте простую гиперссылку, чтобы продемонстрировать свойство
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Сохраните книгу
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


