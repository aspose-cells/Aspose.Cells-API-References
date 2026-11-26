---
title: "AutoFilter.MatchBlanks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Выбирает все пустые ячейки в списке"
type: docs
url: /ru/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Соответствует всем пустым ячейкам в списке.

```csharp
public void MatchBlanks(int fieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные с некоторыми пустыми ячейками
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Оставьте C2 пустой
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Оставьте B3 пустой
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Фильтр, показывающий только строки с пустыми ячейками в столбце 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Обновить фильтр
            filter.Refresh();
            
            // Сохраните книгу
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


