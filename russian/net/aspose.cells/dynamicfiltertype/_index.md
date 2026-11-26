---
title: "Перечисление DynamicFilterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DynamicFilterType. Тип динамического фильтра"
type: docs
url: /ru/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Тип динамического фильтра.

```csharp
public enum DynamicFilterType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| AboveAverage | `0` | Показывает значения, превышающие среднее. |
| BelowAverage | `1` | Показывает значения, ниже среднего. |
| LastMonth | `2` | Показывает даты прошлого месяца. |
| LastQuarter | `3` | Показывает даты последнего квартала. |
| LastWeek | `4` | Показывает даты прошлой недели. |
| LastYear | `5` | Показывает даты прошлого года. |
| January | `6` | Показывает даты, находящиеся в январе, независимо от года. |
| October | `7` | Показывает даты, которые находятся в октябре, независимо от года. |
| November | `8` | Показывает даты, которые находятся в ноябре, независимо от года. |
| December | `9` | Показывает даты, которые находятся в декабре, независимо от года. |
| February | `10` | Показывает даты, которые находятся в феврале, независимо от года. |
| March | `11` | Показывает даты, которые находятся в марте, независимо от года. |
| April | `12` | Показывает даты, которые находятся в апреле, независимо от года. |
| May | `13` | Показывает даты, которые находятся в мае, независимо от года. |
| June | `14` | Показывает даты, которые находятся в июне, независимо от года. |
| July | `15` | Показывает даты, которые находятся в июле, независимо от года. |
| August | `16` | Показывает даты, которые находятся в августе, независимо от года. |
| September | `17` | Показывает даты, которые находятся в сентябре, независимо от года. |
| NextMonth | `18` | Показывает даты следующего месяца. |
| NextQuarter | `19` | Показывает даты следующего квартала. |
| NextWeek | `20` | Показывает даты следующей недели. |
| NextYear | `21` | Показывает даты следующего года. |
| None | `22` | Нет. |
| Quarter1 | `23` | Показывает даты, которые находятся в 1‑м квартале, независимо от года. |
| Quarter2 | `24` | Показывает даты, которые находятся во 2‑м квартале, независимо от года. |
| Quarter3 | `25` | Показывает даты, которые находятся в 3‑м квартале, независимо от года. |
| Quarter4 | `26` | Показывает даты, которые находятся в 4‑м квартале, независимо от года. |
| ThisMonth | `27` | Показывает даты текущего месяца. |
| ThisQuarter | `28` | Показывает даты текущего квартала. |
| ThisWeek | `29` | Показывает даты текущей недели. |
| ThisYear | `30` | Показывает даты текущего года. |
| Today | `31` | Показывает даты сегодняшнего дня. |
| Tomorrow | `32` | Показывает даты завтрашнего дня. |
| YearToDate | `33` | Показывает даты от начала года до сегодняшнего дня включительно. |
| Yesterday | `34` | Показывает даты вчерашнего дня. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Применить автофильтр к листу
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Применить динамический фильтр, чтобы показывать только даты в марте
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Сохраните книгу
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Выведите результаты
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


