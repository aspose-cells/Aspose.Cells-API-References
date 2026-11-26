---
title: "Перечисление CalculationPrecisionStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.CalculationPrecisionStrategy перечисление. Перечисляет стратегии обработки точности вычислений. Из‑за проблемы точности арифметики с плавающей точкой IEEE 754 некоторые, казалось бы, простые формулы могут не вычисляться до ожидаемого результата. Например, формула 0.450.430.02 при вычислении операндов оператором напрямую дает результат, отличный от нуля. Для таких проблем точности некоторые специальные стратегии могут дать ожидаемый результат."
type: docs
url: /ru/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Перечисляет стратегии обработки точности вычислений. Из‑за проблемы точности арифметики с плавающей запятой IEEE 754 некоторые "на первый взгляд простые" формулы могут вычисляться не так, как ожидается. Например, формула "=-0.45+0.43+0.02", при прямом вычислении операндов оператором '+' дает результат, отличный от нуля. Для подобных проблем точности некоторые специальные стратегии могут обеспечить ожидаемый результат.

```csharp
public enum CalculationPrecisionStrategy
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Стратегия не применяется при вычислениях. При вычислении просто используйте оригинальное значение double в качестве операнда и возвращайте результат напрямую. Наиболее эффективно по производительности и применимо в большинстве случаев. |
| Round | `1` | Округляет результат вычисления в соответствии со значимыми цифрами. |
| Decimal | `2` | Использует тип decimal в качестве операндов, когда это возможно. Наименее эффективно по производительности. |

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Установите параметры расчёта
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Вычислить формулы в рабочем листе.
            workbook.CalculateFormula(calcOptions);

            // Получить результат формулы.
            double result = worksheet.Cells["A2"].DoubleValue;

            // Вывести результат.
            Console.WriteLine("Calculated Result: " + result);

            // Сохраните книгу
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


