---
title: "AutoFilter.AddFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет фильтр для столбца фильтра"
type: docs
url: /ru/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Добавляет фильтр для столбца фильтра.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| критерий | String | Указанный критерий (строка; например, "101"). Он может быть только null или значением одной из ячеек в этом столбце. |

### Примечания

MS Excel 2007 поддерживает множественный выбор в столбце фильтра.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Создать диапазон автофильтра
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Получить автофильтр
            AutoFilter filter = worksheet.AutoFilter;
            
            // Добавить фильтры для значений, начинающихся с 'A' и 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Обновить фильтр
            filter.Refresh();
            
            // Сохраните книгу
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


