---
title: "RevisionInsertDelete.ActionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertDelete. Возвращает тип действия этой правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Получает тип действия этой ревизии.

```csharp
public RevisionActionType ActionType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу Workbook и включите отслеживание правок
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Выполните операции, чтобы сгенерировать правки вставки/удаления
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Получить журналы ревизий
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Итерируйте все журналы правок, чтобы найти правки вставки/удаления
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Отобразите значение свойства ActionType
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Продемонстрировать различные типы действий
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Показать связанную информацию
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Сохранить книгу с ревизиями
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


