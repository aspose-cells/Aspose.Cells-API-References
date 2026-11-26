---
title: "BuiltInDocumentPropertyCollection.Pages"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Представляет оценку количества страниц в документе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/pages/
---
## BuiltInDocumentPropertyCollection.Pages property

Представляет оценку количества страниц в документе.

```csharp
public int Pages { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установите свойство Pages
            builtInProperties.Pages = 10;

            // Добавьте лист и некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page Count Demonstration");
            worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");

            // Сохраните книгу
            workbook.Save("DocumentPagesDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


