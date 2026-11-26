---
title: "WorksheetCollection.ExternalLinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Представляет внешние ссылки в книге"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Представляет внешние ссылки в книге.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Создать исходную книгу с внешней ссылкой
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Создайте целевую книгу
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Установить внешний источник данных ссылки
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Сохраните книгу
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Очистить
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### См. также

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


