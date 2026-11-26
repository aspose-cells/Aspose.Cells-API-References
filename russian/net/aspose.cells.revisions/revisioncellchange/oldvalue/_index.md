---
title: "RevisionCellChange.OldValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "RevisionCellChange property. Получает старое значение ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Получает старое значение ячейки.

```csharp
public object OldValue { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить начальные данные для создания ревизии
            worksheet.Cells["A1"].PutValue("Original Value");

            // Измените ячейку, чтобы создать ревизию
            worksheet.Cells["A1"].PutValue("Modified Value");

            try
            {
                // Получите доступ к журналам ревизий
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Отобразить значение свойства OldValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Продемонстрировать использование свойства OldValue
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionCellChangePropertyOldValueDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


