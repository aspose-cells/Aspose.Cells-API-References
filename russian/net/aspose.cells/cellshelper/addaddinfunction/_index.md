---
title: "CellsHelper.AddAddInFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Добавить функцию дополнения"
type: docs
url: /ru/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Добавить функцию дополнения.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| функция | String | Имя функции. |
| minCountOfParameters | Int32 | Минимальное количество параметров, требуемое этой функцией |
| maxCountOfParameters | Int32 | Максимальное количество параметров, разрешённое этой функцией. |
| paramersType | ParameterType[] | Ожидаемый тип параметров функции |
| functionValueType | ParameterType | Тип значения функции. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте методы WorksheetCollection.RegisterAddInFunction(). Этот метод будет удалён через 12 месяцев, начиная с января 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Определить параметры для AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Вызвать метод AddAddInFunction
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Использовать пользовательскую функцию в ячейке
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Вычислить формулы
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


