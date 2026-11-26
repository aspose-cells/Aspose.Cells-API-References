---
title: "AutoFilter.FilterTop10"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Фильтровать 10 лучших элементов в списке"
type: docs
url: /ru/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Отфильтровать 10 лучших элементов в списке

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| isTop | Boolean | Указывает, применяется ли фильтр сверху или снизу |
| isPercent | Boolean | Указывает, являются ли элементы процентами или количеством |
| itemCount | Int32 | Количество элементов |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные (5 строк × 3 столбца с числовыми значениями)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Установить диапазон автофильтра
            worksheet.AutoFilter.Range = "A1:A6";

            // Применить фильтр топ‑10 (показывая 2 лучших элемента)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Обновить фильтр
            worksheet.AutoFilter.Refresh();

            // Сохраните книгу
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


