---
title: "Класс Top10"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Top10. Описание правила условного форматирования Top10. Это правило условного форматирования выделяет ячейки, значения которых находятся в верхнем N или нижнем N диапазоне, как указано."
type: docs
url: /ru/net/aspose.cells/top10/
---
## Top10 class

Опишите правило условного форматирования Top10. Это правило условного форматирования выделяет ячейки, значения которых находятся в верхних N или нижних N диапазонах, как указано.

```csharp
public class Top10
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Top10](top10/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Получить или установить, является ли правило "top/bottom n" правилом "bottom n". Значение по умолчанию — false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Получить или установить, является ли правило "top/bottom n" правилом "top/bottom n percent". Значение по умолчанию — false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Получить или установить значение "n" в правиле условного форматирования "top/bottom n". Если IsPercent равно true, значение должно быть от 0 до 100. В противном случае оно должно быть от 0 до 1000. Значение по умолчанию — 10. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Добавляет условие
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Установка свойств
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Сохранение файла Excel
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


