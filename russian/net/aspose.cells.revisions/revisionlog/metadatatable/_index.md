---
title: "RevisionLog.MetadataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionLog. Возвращает таблицу, содержащую метаданные о списке конкретных изменений, произошедших в этом workbook"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Получает таблицу, содержащую метаданные о списке конкретных изменений, произошедших в этой книге.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Внесите некоторые изменения, чтобы создать историю ревизий
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Измените ячейку, чтобы создать ревизию
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Откройте заново изменённый workbook, чтобы получить доступ к журналам ревизий
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### См. также

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


