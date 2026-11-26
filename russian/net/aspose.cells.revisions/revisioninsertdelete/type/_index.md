---
title: "RevisionInsertDelete.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertDelete. Представляет тип правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

Представляет тип ревизии.

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

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу Workbook и включите отслеживание правок
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Вставьте строку, чтобы создать запись правки
            worksheet.Cells.InsertRows(0, 1);

            // Получите коллекцию правок (RevisionLogCollection сама является коллекцией)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Найдите RevisionInsertDelete среди правок
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Отобразите значение свойства Type
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Продемонстрировать использование свойства Type
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


