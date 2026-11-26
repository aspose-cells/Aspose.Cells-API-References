---
title: "CalculationOptions.CustomEngine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Пользовательский движок вычисления формул, расширяющий движок вычислений по умолчанию в Aspose.Cells"
type: docs
url: /ru/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Пользовательский движок вычисления формул для расширения движка расчётов по умолчанию в Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCustomEngineDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Установить формулу HYPERLINK в ячейку A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Создать пользовательский движок, обрабатывающий функцию HYPERLINK
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Установить параметры вычисления с пользовательским движком
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Вычислите формулы с пользовательским движком
            wb.CalculateFormula(options);
            
            Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
        }
    }

    public class CustomEngineForHyperlink : AbstractCalculationEngine
    {
        public bool Invoked { get; private set; }
        private readonly bool _shouldProcess;

        public CustomEngineForHyperlink(bool shouldProcess)
        {
            _shouldProcess = shouldProcess;
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "HYPERLINK" && _shouldProcess)
            {
                Invoked = true;
                data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
            }
            // Не вызывайте base.Calculate(), так как он абстрактный
            // Просто позвольте выполнить расчёт по умолчанию для остальных функций
        }
    }
}
```

### См. также

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


