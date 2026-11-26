---
title: "RevisionCellMove.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellMove. Представляет тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

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

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Создайте экземпляр RevisionCellMove с помощью рефлексии
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Отобразите значение свойства Type (только для чтения)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Показать дополнительный контекст (необязательно)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Сохраните книгу (необязательно)
                workbook.Save("RevisionCellMoveTypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


