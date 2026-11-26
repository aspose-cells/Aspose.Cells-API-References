---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractCalculationEngine. Нужно ли принудительно пересчитывать данную функцию каждый раз при вычислении общих формул"
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Определяет, следует ли принудительно всегда пересчитывать данную функцию при вычислении общих формул.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| functionName | String | имя функции. Обычно это имя пользовательской функции. Если [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) равно true, то встроенные функции также будут проверяться здесь. |

### Возвращаемое значение

true, если указанную функцию необходимо пересчитывать каждый раз.

### Примечания

Для общих формул несколько ячеек используют одну и ту же функцию. Если параметры функции остаются одинаковыми для этих ячеек, то обычно эту функцию нужно вычислять только один раз. Поэтому из соображений производительности мы также вычисляем такой тип функции один раз ([`Calculate`](../calculate/) вызывается только один раз, вместо многократных вызовов для каждой ячейки). Однако в пользовательской реализации функция, особенно пользовательская функция, может требовать различного вычисления для разных ячеек. В этом случае пользователь должен переопределить этот метод, чтобы он возвращал true для функции. И для [`Calculate`](../calculate/) переданный [`CalculatedValue`](../../calculationdata/calculatedvalue/) может быть инициализирован кэшированным значением предыдущего вычисления.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### См. также

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


