---
title: "RevisionAutoFormat.CellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionAutoFormat. Получает место, где было применено форматирование"
type: docs
url: /ru/net/aspose.cells.revisions/revisionautoformat/cellarea/
---
## RevisionAutoFormat.CellArea property

Получает расположение, где было применено форматирование.

```csharp
public CellArea CellArea { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyCellAreaDemo
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
                    // Продемонстрируйте свойство CellArea (только для чтения)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


