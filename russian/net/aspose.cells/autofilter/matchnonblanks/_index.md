---
title: "AutoFilter.MatchNonBlanks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Выбирает все непустые ячейки в списке"
type: docs
url: /ru/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Соответствует всем непустым ячейкам в списке.

```csharp
public void MatchNonBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные с некоторыми пустыми ячейками
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // Примените автофильтр, чтобы показывать только непустые ячейки в столбце A (индекс 0)
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Сохраните книгу
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


