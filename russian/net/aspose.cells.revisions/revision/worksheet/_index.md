---
title: "Revision.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Revision. Получает рабочий лист"
type: docs
url: /ru/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Получает лист.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить свойства листа
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Добавьте данные, чтобы продемонстрировать ревизии
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Защитите рабочий лист, чтобы включить отслеживание изменений
            worksheet.Protect(ProtectionType.All);
            
            // Сделайте изменение, которое будет отслеживаться как ревизия
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Сохраните рабочую книгу, чтобы отслеживать ревизии
            workbook.Save("RevisionDemo.xlsx");
            
            // Загрузите рабочую книгу с ревизиями
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Получите доступ к журналам ревизий
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Продемонстрировать доступ к свойству Worksheet из ревизии
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


