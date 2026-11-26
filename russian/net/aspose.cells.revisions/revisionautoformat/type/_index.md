---
title: "RevisionAutoFormat.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionAutoFormat. Получает тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

Получает тип ревизии.

```csharp
public override RevisionType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к коллекции журналов ревизий
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // Найдите первый экземпляр RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Продемонстрируйте свойство Type (только для чтения)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");
                    
                    // Отобразите значение перечисления для ясности
                    Console.WriteLine($"Revision type value: {(int)type}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


