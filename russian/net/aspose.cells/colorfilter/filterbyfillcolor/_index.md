---
title: "ColorFilter.FilterByFillColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorFilter. Определяет, фильтровать ли по цвету заливки ячеек"
type: docs
url: /ru/net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Фильтровать по цвету заливки ячейки.

```csharp
public bool FilterByFillColor { get; set; }
```

### Примечания

True: цвет заливки ячейки; False: цвет шрифта ячейки.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterPropertyFilterByFillColorDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить примерные данные с разными цветами заливки
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");

            // Установить цвета заливки
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);

            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);

            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;

            // Создать цветовой фильтр для заливки
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
            filter.Refresh();

            // Проверить настройки фильтра
            FilterColumn filterColumn = filter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            // Продемонстрировать свойство FilterByFillColor
            Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
            Console.WriteLine("Filtered rows:");
            for (int row = 1; row <= 3; row++)
            {
                Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
            }
        }
    }
}
```

### См. также

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


