---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Справочник API Aspose.Cells для .NET"
description: "BuiltInDocumentPropertyCollection свойство. Получает или задает свойство гиперссылки"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Получает или задает свойство hyperlinkbase.

```csharp
public string HyperlinkBase { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установите свойство HyperlinkBase
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Установите другое свойство для демонстрации
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Сохраните книгу
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Выведите свойства в консоль
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


