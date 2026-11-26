---
title: "FilterColumn.Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает и задаёт условие фильтрации данных"
type: docs
url: /ru/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Получает и задаёт условие фильтрации данных.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте соответствующее свойство согласно [`FilterType`](../filtertype/). И для типа фильтра MultipleFilters возвращаемый объект теперь является [`FilterValueCollection`](../../filtervaluecollection/), а не [`MultipleFilterCollection`](../../multiplefiltercollection/). Это свойство будет удалено через 12 месяцев, начиная с октября 2025 года. Компания Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные с цветовым форматированием
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Форматировать ячейки цветами
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Добавить цветовой фильтр для красных ячеек
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Получить доступ к столбцу фильтра и его свойству Filter
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Вывести свойства фильтра
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Сохраните книгу
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


