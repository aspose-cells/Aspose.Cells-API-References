---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractCalculationEngine. Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке."
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке.

```csharp
public void SkipCalculation()
```

### Примечания

Этот метод может быть вызван в реализации [`Calculate`](../calculate/), чтобы пропустить вычисление всей формулы, и исходное значение формулы будет сохранено без изменений.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Создать пользовательский движок расчёта
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Вычислите рабочую книгу, что запустит наш пользовательский движок
                workbook.CalculateFormula(options);

                // Отобразить результат (должен быть пропущен)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Сохраните книгу
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Пропустить вычисление этой формулы
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### См. также

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


