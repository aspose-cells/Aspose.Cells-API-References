---
title: "AutoFilter.Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Фильтрует список по указанным критериям"
type: docs
url: /ru/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Фильтрует список с указанными критериями.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| критерий | String | Указанный критерий (строка; например, "101"). |

### Примечания

Aspose.Cells удалит все остальные настройки фильтра для этого поля, как в MS Excel 97-2003.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Примените автофильтр, используя правильные параметры SetRange
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Сохранить результат
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


