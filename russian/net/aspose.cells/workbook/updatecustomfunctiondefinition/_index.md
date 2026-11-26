---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Обновляет определение пользовательских функций"
type: docs
url: /ru/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Обновляет определение пользовательских функций.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| определение | CustomFunctionDefinition | Особое определение пользовательских функций для специальных требований пользователя. |

### Примечания

Этот метод может использоваться в некоторых специальных сценариях. Например, если пользователю нужны параметры некоторых пользовательских функций, вычисляемые в режиме массива, он может предоставить собственное определение с реализованным [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) для этих функций. После обновления данных формул указанные параметры будут автоматически вычисляться в режиме массива при расчёте соответствующих пользовательских функций.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Создать пользовательский движок расчёта
            var customEngine = new MyCustomCalculationEngine();
            
            // Установить параметры вычисления с пользовательским движком
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Обновить определение пользовательской функции
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Установить формулу с использованием пользовательской функции
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Вычислить формулы
            wb.CalculateFormula(options);

            // Вывести результат.
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Вернуть индексы параметров, которые должны обрабатываться в режиме массива
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### См. также

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


