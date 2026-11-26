---
title: "Перечисление FormatConditionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FormatConditionType. Тип правила условного форматирования"
type: docs
url: /ru/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Тип правила условного форматирования.

```csharp
public enum FormatConditionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| CellValue | `1` | Это правило условного форматирования сравнивает значение ячейки с результатом вычисленной формулы, используя оператор. |
| Expression | `2` | Это правило условного форматирования содержит формулу для вычисления. Когда результат формулы истинный, ячейка выделяется. |
| Top10 | `4` | Это правило условного форматирования выделяет ячейки, значения которых попадают в верхний N или нижний N диапазон, как указано. |
| UniqueValues | `8` | Это правило условного форматирования выделяет уникальные значения в диапазоне. |
| DuplicateValues | `16` | Это правило условного форматирования выделяет дублированные значения. |
| ContainsText | `32` | Это правило условного форматирования выделяет ячейки, содержащие заданный текст. Эквивалентно использованию функции листа SEARCH() для определения, содержит ли ячейка текст. |
| NotContainsText | `64` | Это правило условного форматирования выделяет ячейки, которые не содержат заданный текст. Эквивалентно использованию функции листа SEARCH() для определения, содержит ли ячейка текст или нет. |
| BeginsWith | `128` | Это правило условного форматирования выделяет ячейки в диапазоне, которые начинаются с заданного текста. Эквивалентно использованию функции листа LEFT() и сравнению значений. |
| EndsWith | `256` | Это правило условного форматирования выделяет ячейки, заканчивающиеся заданным текстом. Эквивалентно использованию функции листа RIGHT() и сравнению значений. |
| ContainsBlanks | `512` | Это правило условного форматирования выделяет ячейки, которые полностью пусты. Эквивалентно использованию LEN(TRIM()). Это означает, что если ячейка содержит только символы, которые удалит TRIM(), она считается пустой. Пустая ячейка также считается пустой. |
| NotContainsBlanks | `1024` | Это правило условного форматирования выделяет ячейки, которые не пусты. Эквивалентно использованию LEN(TRIM()). Это означает, что если ячейка содержит только символы, которые удалит TRIM(), она считается пустой. Пустая ячейка также считается пустой. |
| ContainsErrors | `2048` | Это правило условного форматирования выделяет ячейки с ошибками формулы. Эквивалентно использованию функции листа ISERROR() для определения наличия ошибки формулы. |
| NotContainsErrors | `4096` | Это правило условного форматирования выделяет ячейки без ошибок формулы. Эквивалентно использованию функции листа ISERROR() для определения наличия ошибки формулы. |
| TimePeriod | `8192` | Это правило условного форматирования выделяет ячейки, содержащие даты в указанном периоде времени. Оценивается базовое значение ячейки, поэтому ячейка не обязана быть отформатирована как дата для оценки. Например, при ячейке со значением 38913 условный формат будет применён, если правило требует значение 14.07.2006. |
| AboveAverage | `16384` | Это правило условного форматирования выделяет ячейки, значения которых выше или ниже среднего для всех значений в диапазоне. |
| ColorScale | `32768` | Это правило условного форматирования создает градуированную цветовую шкалу в ячейках. |
| DataBar | `65536` | Это правило условного форматирования отображает градуированную полоску данных в диапазоне ячеек. |
| IconSet | `131072` | Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Создайте новую Workbook.
            Workbook workbook = new Workbook();

            // Получите первый worksheet.
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Добавляет условие для AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Установка свойств для AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Добавляет условие для CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Добавляет условие для ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Сохраните файл Excel
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


