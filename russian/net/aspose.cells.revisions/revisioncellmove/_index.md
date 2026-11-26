---
title: "Класс RevisionCellMove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.RevisionCellMove класс. Представляет запись ревизии о перемещённой ячейке"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellmove/
---
## RevisionCellMove class

Представляет запись ревизии о перемещении ячейки(й).

```csharp
public class RevisionCellMove : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DestinationArea](../../aspose.cells.revisions/revisioncellmove/destinationarea/) { get; } | Получает целевую область. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [SourceArea](../../aspose.cells.revisions/revisioncellmove/sourcearea/) { get; } | Получает исходную область. |
| [SourceWorksheet](../../aspose.cells.revisions/revisioncellmove/sourceworksheet/) { get; } | Получает исходный лист. |
| override [Type](../../aspose.cells.revisions/revisioncellmove/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellMoveDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте экземпляр класса RevisionCellMove с помощью рефлексии
                // поскольку конструктор недоступен напрямую
                RevisionCellMove revisionCellMove = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Отобразите свойства только для чтения
                Console.WriteLine("Revision Type: " + revisionCellMove.Type);
                Console.WriteLine("Source Area: " + revisionCellMove.SourceArea);
                Console.WriteLine("Destination Area: " + revisionCellMove.DestinationArea);

                // Проверьте, доступен ли SourceWorksheet
                if (revisionCellMove.SourceWorksheet != null)
                {
                    Console.WriteLine("Source Worksheet: " + revisionCellMove.SourceWorksheet.Name);
                }
                else
                {
                    Console.WriteLine("Source Worksheet: null");
                }

                // Сохраните книгу
                workbook.Save("RevisionCellMoveDemo.xlsx");
                Console.WriteLine("RevisionCellMove demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionCellMove: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


