---
title: "Перечисление IconSetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.IconSetType. Тип набора значков для условного форматирования. Пороговые значения для срабатывания разных значков в наборе настраиваемы, а порядок значков обратим."
type: docs
url: /ru/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Тип набора значков для условного форматирования. Пороговые значения для активации различных значков в наборе настраиваемы, и порядок значков можно изменить.

```csharp
public enum IconSetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Arrows3 | `0` | Набор значков из 3 стрелок. |
| ArrowsGray3 | `1` | Набор значков из 3 серых стрелок. |
| Flags3 | `2` | Набор значков из 3 флагов. |
| Signs3 | `3` | Набор значков из 3 знаков. |
| Symbols3 | `4` | Набор значков из 3 символов (в кружке). |
| Symbols32 | `5` | Набор значков из 3 символов (без круга). |
| TrafficLights31 | `6` | Набор значков из 3 светофоров (без рамки). |
| TrafficLights32 | `7` | Набор значков из 3 светофоров с толстой чёрной рамкой. |
| Arrows4 | `8` | Набор значков из 4 стрелок. |
| ArrowsGray4 | `9` | Набор значков из 4 серых стрелок. |
| Rating4 | `10` | Набор значков из 4 рейтингов. |
| RedToBlack4 | `11` | Набор значков из 4 «от красного к чёрному». |
| TrafficLights4 | `12` | Набор значков из 4 светофоров. |
| Arrows5 | `13` | Набор иконок из 5 стрелок. |
| ArrowsGray5 | `14` | Набор иконок из 5 серых стрелок. |
| Quarters5 | `15` | Набор иконок из 5 четвертей. |
| Rating5 | `16` | Набор иконок для оценки из 5 элементов. |
| Stars3 | `17` | Набор из 3 звёзд |
| Boxes5 | `18` | Набор из 5 коробок |
| Triangles3 | `19` | Набор из 3 треугольников |
| None | `20` | Нет |
| CustomSet | `21` | CustomSet. Этот элемент только для чтения. |
| Smilies3 | `22` | 3 смайлика. Только для .ods. |
| ColorSmilies3 | `23` | 3 цветных смайлика. Только для .ods. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить примерные значения
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Добавить условное форматирование с набором иконок
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Получить и отобразить результаты
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


