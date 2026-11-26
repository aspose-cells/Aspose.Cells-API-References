---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает общее время редактирования в минутах"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

Получает или задает общее время редактирования в минутах.

```csharp
public double TotalEditingTime { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установить общее время редактирования в минутах
            builtInProperties.TotalEditingTime = 90.5;

            // Отобразить установленное время редактирования
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // Сохраните книгу
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


