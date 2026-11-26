---
title: "DataSorter.AddColorKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DataSorter. Добавляет ключ сортировки по цвету"
type: docs
url: /ru/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Добавляет ключ сортировки по цвету.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | Int32 | Индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...) |
| type | SortOnType | Тип отсортированного значения цвета. |
| порядок | SortOrder | Порядок сортировки. |
| цвет | Color | Пользовательский цвет сортировки. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с раскрашенными ячейками
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Применить цвета к ячейкам
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Создать сортировщик данных и добавить цветовой ключ
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Отсортировать данные
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Вывести отсортированные значения (для демонстрации)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### См. также

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


