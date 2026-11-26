---
title: "RevisionInsertDelete.Revisions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertDelete. Получает список ревизий для этой операции"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertdelete/revisions/
---
## RevisionInsertDelete.Revisions property

Получает список ревизий по этой операции.

```csharp
public RevisionCollection Revisions { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyRevisionsDemo
    {
        public static void Run()
        {
            // Создайте новую книгу Workbook и включите отслеживание правок
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Выполнить операции для создания ревизий
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteRows(1, 1);

            // Получить журналы ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Перебрать все журналы ревизий
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Получить доступ к свойству Revisions (только для чтения)
                        RevisionCollection revisions = revisionInsertDelete.Revisions;

                        // Отобразить информацию о ревизиях
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
                        Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
                        Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
                        Console.WriteLine("Number of related revisions: " + revisions.Count);

                        // Продемонстрировать использование коллекции Revisions
                        foreach (Revision relatedRevision in revisions)
                        {
                            Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
                            if (relatedRevision is RevisionInsertDelete)
                            {
                                RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
                                Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
                                Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
                            }
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


