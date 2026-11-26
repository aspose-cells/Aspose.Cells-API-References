---
title: "CalculationData.CalculatedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает или задаёт рассчитанное значение для этой функции"
type: docs
url: /ru/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Получает или задаёт вычисленное значение для этой функции.

```csharp
public object CalculatedValue { get; set; }
```

### Примечания

Пользователь должен установить это свойство в своём пользовательском движке расчёта для тех функций, которые поддерживает движок, и установленное значение будет возвращено при последующем получении свойства. Установленное значение может быть одним из возможных типов [`Value`](../../cell/value/), массивом таких значений, либо объектом Range, Name, ReferredArea. Получение этого свойства до установки значения приведёт к вычислению функции стандартным движком расчёта Aspose.Cells, после чего будет возвращено рассчитанное значение (обычно это будет #NAME? для пользовательских функций).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Создать параметры расчёта с пользовательским движком
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Вычислить формулы с параметрами
            workbook.CalculateFormula(options);

            // Получить рассчитанное значение
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


