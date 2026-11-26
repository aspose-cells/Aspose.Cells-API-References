---
title: "RevisionCellChange.NewValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Возвращает новое значение ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/newvalue/
---
## RevisionCellChange.NewValue property

Получает новое значение ячейки.

```csharp
public object NewValue { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте начальные данные в ячейку A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");

            // Измените ячейку, чтобы создать ревизию
            cell.PutValue("Modified Value");

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
                            // Отобразите свойство NewValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Продемонстрируйте использование свойства NewValue
                            if (cellChange.NewValue != null)
                            {
                                Console.WriteLine("\nThe new value is: " + cellChange.NewValue.ToString());
                            }
                        }
                    }
                }

                // Сохранить книгу с ревизиями
                workbook.Save("RevisionCellChangePropertyNewValueDemo.xlsx");
                Console.WriteLine("\nWorkbook saved with revisions.");
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


