---
title: "RevisionCellChange.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Представляет тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/type/
---
## RevisionCellChange.Type property

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

    public class RevisionCellChangePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить отслеживание изменений, изменяя ячейку — ревизии отслеживаются автоматически
            // когда изменения вносятся после создания книги
            Cell cell = worksheet.Cells["A1"];
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
                        // Отобразить информацию о типе из ревизии
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Revision Type: " + cellChange.Type);

                        // Продемонстрировать использование свойства Type
                        if (cellChange.Type == RevisionType.ChangeCells)
                        {
                            Console.WriteLine("\nThis is a cell change revision");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }

                        // Проверить другие возможные типы ревизий
                        switch (cellChange.Type)
                        {
                            case RevisionType.ChangeCells:
                                Console.WriteLine("Handling cell value change revision");
                                break;
                            case RevisionType.Format:
                                Console.WriteLine("Handling format change revision");
                                break;
                            default:
                                Console.WriteLine("Handling other type of revision");
                                break;
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


