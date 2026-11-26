---
title: "RevisionCellChange.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "RevisionCellChange property. Получает индекс столбца ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Получает индекс столбца ячейки.

```csharp
public int Column { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Изменить ячейку B2, чтобы создать ревизию
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Initial Value");

            // Измените ячейку, чтобы создать ревизию
            cell.PutValue("Modified Value");

            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Отобразить информацию о столбце из ревизии
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Продемонстрировать использование свойства Column
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


