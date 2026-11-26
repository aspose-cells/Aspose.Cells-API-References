---
title: "RevisionLog.Revisions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionLog. Возвращает все исправления в этом журнале"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Получает все ревизии в этом журнале.

```csharp
public RevisionCollection Revisions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyRevisionsDemo
    {
        public static void Run()
        {
            // Создать книгу с историей исправлений
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Внести некоторые изменения для отслеживания исправлений
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Сохранить с отслеживанием исправлений
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Внести дополнительные изменения для создания исправлений
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Сохранить снова, чтобы зафиксировать исправления
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Загрузите рабочую книгу с ревизиями
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Обработать каждый журнал исправлений
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Получить доступ к коллекции исправлений
                RevisionCollection revisions = log.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


