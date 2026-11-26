---
title: "BuiltInDocumentPropertyCollection.LastPrintedUniversalTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает универсальное время последней печати документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinteduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property

Получает или задает универсальное время последней печати документа.

```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установить свойство LastPrintedUniversalTime
            DateTime currentUtcTime = DateTime.UtcNow;
            builtInProperties.LastPrintedUniversalTime = currentUtcTime;

            // Отобразить установленное значение
            Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);

            // Сохраните книгу
            workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


