---
title: "PaneCollection.AcitvePaneType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaneCollection. Получает и задает активную область"
type: docs
url: /ru/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Получает и задает активную панель.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство [`ActivePaneType`](../activepanetype/) property. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные, чтобы продемонстрировать разделение областей
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Разделите лист на области
            worksheet.Split();

            // Получить коллекцию областей
            PaneCollection panes = worksheet.GetPanes();

            // Отобразить текущую активную область
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Установить активную область в BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Установить первую видимую строку/столбец для нижних/правых областей
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Сохраните книгу
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


