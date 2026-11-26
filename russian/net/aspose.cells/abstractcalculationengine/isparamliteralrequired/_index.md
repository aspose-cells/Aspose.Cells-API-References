---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractCalculationEngine. Указывает, требуется ли этому движку буквальный текст параметра при выполнении вычисления. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Указывает, требуется ли этому движку буквальный текст параметра при выполнении расчёта. Значение по умолчанию — false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Примечания

Если этому пользовательскому движку вычислений требуется буквальный текст параметра, понадобится больше стеков для кэширования буквального текста параметров, и метод Calculate() может вызываться рекурсивно для вычисления значения параметра. Как правило, буквальный текст не нужен для вычисления формул, и это свойство следует оставлять false в большинстве реализаций для повышения производительности.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamLiteralRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр пользовательского движка вычислений
            MyCustomEngine engine = new MyCustomEngine();

            // Прочитать текущее значение свойства
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Создать тестовую формулу со строковым литеральным параметром
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Вычислить рабочую книгу с пользовательскими параметрами расчёта
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Показать результат расчёта на основе значения свойства
            Console.WriteLine("Formula result: " + worksheet.Cells["A1"].StringValue);

            workbook.Save("IsParamLiteralRequiredDemo.xlsx");
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override bool IsParamLiteralRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
            {
                if (data.ParamCount > 0)
                {                    
                    object paramValue = data.GetParamValue(0);
                    string result = (paramValue is string) ? "Literal received" : "Value received";
                    data.CalculatedValue = result;
                }
            }
        }
    }
}
```

### См. также

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


