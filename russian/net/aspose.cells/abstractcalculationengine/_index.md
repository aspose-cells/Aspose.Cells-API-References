---
title: "Класс AbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AbstractCalculationEngine. Представляет пользовательский движок расчётов, расширяющий движок расчётов по умолчанию в Aspose.Cells"
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false. Если при расчёте пользовательских функций требуется [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) и пользователь не обновил их определение (с помощью [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), это свойство должно быть установлено в true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Указывает, требуется ли этому движку буквальный текст параметра при выполнении расчёта. Значение по умолчанию — false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией. По умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Вычисляет одну функцию с заданными данными. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Определяет, следует ли принудительно всегда пересчитывать данную функцию при вычислении общих формул. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке. |

### Примечания

Пользователь не должен изменять любую часть Workbook напрямую в этой реализации (за исключением вычисленного результата пользовательской функции, который можно задать через свойство CalculationData.CalculatedValue). В противном случае могут возникнуть неожиданные результаты или Exception. Если пользователю необходимо изменить данные, отличные от вычисленного результата, в реализации некоторых пользовательских функций, например, изменить формулу ячейки, стиль и т.д., пользователь должен собрать эти данные в этой реализации и изменить их вне области вычисления формул.

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Пример: пользовательская реализация функции с именем "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Предположим, что MYFUNC принимает два параметра и возвращает их сумму
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Принудительно пересчитать пользовательскую функцию "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Поместите некоторые значения в ячейки
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Добавьте формулу, использующую пользовательскую функцию
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Установите параметры расчёта с помощью пользовательского движка
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Вычислите формулы с пользовательским движком
            workbook.CalculateFormula(options);

            // Выведите результат пользовательской функции
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Сохраните книгу
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


