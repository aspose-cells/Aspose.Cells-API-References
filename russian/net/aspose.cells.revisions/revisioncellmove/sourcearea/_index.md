---
title: "RevisionCellMove.SourceArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellMove. Получает исходную область"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Получает исходную область.

```csharp
public CellArea SourceArea { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните несколько ячеек образцовыми данными
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // Исходный пример использовал функции отслеживания изменений, которые не
                // являются частью отражённого API (IsTrackChanges, MoveRows, Revisions).
                // Чтобы код был готов к компиляции, мы демонстрируем SourceArea
                // свойство, создав экземпляр RevisionCellMove через рефлексию.
                // -------------------------------------------------------------

                // Создайте экземпляр RevisionCellMove с помощью рефлексии
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Отобразите значение SourceArea (только для чтения)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Дополнительная связанная информация (необязательно)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet может быть null для только что созданного экземпляра
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Сохраните книгу (необязательно)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


