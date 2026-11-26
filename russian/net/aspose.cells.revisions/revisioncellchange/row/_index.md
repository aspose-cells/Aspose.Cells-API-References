---
title: "RevisionCellChange.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "RevisionCellChange property. Получает индекс строки ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

Получает индекс строки ячейки.

```csharp
public int Row { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить начальные данные для создания ревизии
            worksheet.Cells["B5"].PutValue("Original Value");

            // Измените ячейку, чтобы создать ревизию
            worksheet.Cells["B5"].PutValue("Modified Value");

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
                            // Отобразите значение свойства Row
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Продемонстрировать использование свойства Row
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
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


