---
title: "Перечисление FilterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FilterType. Тип фильтра"
type: docs
url: /ru/net/aspose.cells/filtertype/
---
## FilterType enumeration

Тип фильтра.

```csharp
public enum FilterType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| ColorFilter | `0` | Фильтрация по цвету заливки ячейки. |
| CustomFilters | `1` | Пользовательский тип фильтра. |
| DynamicFilter | `2` | Тип динамического фильтра. |
| MultipleFilters | `3` | Когда выбирается несколько значений для фильтрации, или когда выбирается группа дат, этот элемент группирует эти критерии вместе. |
| IconFilter | `4` | Фильтрация по значку условного форматирования. |
| Top10 | `5` | Фильтр Top 10. |
| None | `6` | Без фильтра. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Создать цветовой фильтр
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Добавить цветовой фильтр в столбец
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Проверить тип фильтра
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Проверить свойства цветового фильтра
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


