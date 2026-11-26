---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionLogCollection. Получает и задает количество дней, в течение которых приложение таблиц будет хранить историю изменений для этой рабочей книги"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Получает и задает количество дней, в течение которых приложение электронных таблиц будет хранить историю изменений для этой книги.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Установите свойство DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Перезагрузите, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### См. также

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


