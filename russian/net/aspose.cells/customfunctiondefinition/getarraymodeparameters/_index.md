---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomFunctionDefinition. Получает индексы параметров заданных пользовательских функций, которые необходимо вычислять в режиме массива"
type: docs
url: /ru/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Получает индексы параметров заданной пользовательской функции, которые необходимо вычислить в режиме массива.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| functionName | String | Имя пользовательской функции. |

### Возвращаемое значение

Индексы параметров, которые необходимо вычислять в режиме массива для заданной пользовательской функции. По умолчанию null, нет параметров, которые нужно вычислять в режиме массива для этой функции.

### Примечания

Для выражения, которое необходимо вычислить, возьмём в качестве примера A:A+B:B: Обычно в режиме значения оно будет вычислено в единственное значение в соответствии с текущей ячейкой. Но в режиме массива будут вычислены все значения A1+B1, A2+B2, A3+B3, ... и использованы для вычисления.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Вызовите GetArrayModeParameters с параметром имени функции
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Отобразить результат
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


