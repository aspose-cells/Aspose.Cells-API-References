---
title: "Перечисление FilterOperatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FilterOperatorType. Пользовательский тип оператора фильтра"
type: docs
url: /ru/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Тип оператора пользовательского фильтра.

```csharp
public enum FilterOperatorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LessOrEqual | `0` | Представляет оператор LessOrEqual. |
| LessThan | `1` | Представляет оператор LessThan. |
| Equal | `2` | Представляет оператор Equal. |
| GreaterThan | `3` | Представляет оператор GreaterThan. |
| NotEqual | `4` | Представляет оператор NotEqual. |
| GreaterOrEqual | `5` | Представляет оператор GreaterOrEqual. |
| None | `6` | Представляет отсутствие сравнения. |
| BeginsWith | `7` | Начинается с текста. |
| EndsWith | `8` | Заканчивается текстом. |
| Contains | `9` | Содержит текст. |
| NotContains | `10` | Не содержит текст. |
| NotBeginsWith | `11` | Не начинается с текста. |
| NotEndsWith | `12` | Не заканчивается текстом. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Установить диапазон автофильтра
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Применить пользовательский фильтр, чтобы показать имена, начинающиеся с "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Обновить фильтр
            worksheet.AutoFilter.Refresh();
            
            // Сохраните книгу
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


