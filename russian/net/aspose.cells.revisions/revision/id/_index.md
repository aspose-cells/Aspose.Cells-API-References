---
title: "Revision.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Revision. Возвращает номер этой ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Получает номер этой ревизии.

```csharp
public int Id { get; }
```

### Примечания

Ноль означает, что эта ревизия не содержит id.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Сделайте изменение, чтобы потенциально создать ревизию
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Получите коллекцию журналов ревизий
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Получите ревизии из первого журнала
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Получите доступ к первой ревизии
                        Revision revision = revisions[0];
                        
                        // Отобразите свойство Id (только для чтения)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Сохраните книгу
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


