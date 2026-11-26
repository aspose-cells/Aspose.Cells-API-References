---
title: "AbstractCalculationEngine.ProcessBuiltInFunctions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractCalculationEngine. Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией. По умолчанию — false."
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/processbuiltinfunctions/
---
## AbstractCalculationEngine.ProcessBuiltInFunctions property

Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией. По умолчанию — false.

```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```

### Примечания

Если пользователю необходимо изменить логику расчёта некоторых встроенных функций, это свойство следует установить в true. В противном случае оставьте его false для повышения производительности.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyProcessBuiltInFunctionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить тестовыми данными
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Создать пользовательские движки расчёта с разными значениями ProcessBuiltInFunctions
            CustomEngine engineProcessEnabled = new CustomEngine(true);
            CustomEngine engineProcessDisabled = new CustomEngine(false);

            // Показать значения свойств
            Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
            Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);

            // Вычислить с пользовательским движком (ProcessBuiltInFunctions = true)
            CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
            workbook.CalculateFormula(optionsEnabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);

            // Вычислить с пользовательским движком (ProcessBuiltInFunctions = false)
            CalculationOptions optionsDisabled = new CalculationOptions { CustomEngine = engineProcessDisabled };
            workbook.CalculateFormula(optionsDisabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=false: " + worksheet.Cells["A4"].Value);

            workbook.Save("ProcessBuiltInFunctionsDemo.xlsx");
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        private readonly bool _processBuiltIn;

        public CustomEngine(bool processBuiltIn)
        {
            _processBuiltIn = processBuiltIn;
        }

        public override bool ProcessBuiltInFunctions => _processBuiltIn;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("SUM", StringComparison.OrdinalIgnoreCase) && ProcessBuiltInFunctions)
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object param = data.GetParamValue(i);
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);

                    for (int r = paramArea1.StartRow; r <= paramArea1.EndRow; r++)
                    {
                        for (int c = paramArea1.StartColumn; c <= paramArea1.EndColumn; c++)
                        {
                            object cellValue = paramArea1.GetValue(r, c);
                            sum += Convert.ToDouble(cellValue);
                        }
                    }
                    
                }
                data.CalculatedValue = sum * 2; // Custom SUM implementation doubles the result
            }
            // Другие функции обрабатываются движком по умолчанию
        }

        public override bool ForceRecalculate(string functionName) => false;
    }
}
```

### См. также

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


