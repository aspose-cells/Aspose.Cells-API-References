---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает дату последней печати документа в локальном часовом поясе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Получает или задает дату последней печати документа в локальном часовом поясе.

```csharp
public DateTime LastPrinted { get; set; }
```

### Примечания

Если документ никогда не печатался, это свойство вернёт DateTime.MinValue.

Aspose.Cells не обновляет это свойство при изменении документа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить встроенные свойства документа
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Отобразить свойство LastPrinted
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


