---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CalculationData. Возвращает значения параметра по заданному индексу. Если параметр представляет собой некоторый тип выражения, требующий вычисления, то он будет вычислен в режиме массива"
type: docs
url: /ru/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Получает значение(я) параметра по заданному индексу. Если параметр представляет собой выражение, которое необходимо вычислить, оно будет вычислено в режиме массива.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс параметра (начиная с 0) |
| maxRowCount | Int32 | Ограничение количества строк для возвращаемого массива. Если оно неположительное или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | Int32 | Ограничение количества столбцов для возвращаемого массива. Если оно неположительное или превышает фактическое количество строк, будет использовано фактическое количество столбцов. |

### Возвращаемое значение

Массив, содержащий все элементы, представленные указанным параметром.

### Примечания

Для выражения, которое необходимо вычислить, возьмём в качестве примера A:A+B:B: в режиме значения оно будет вычислено в одно значение в соответствии с текущей базой ячейки. Но в режиме массива все значения A1+B1, A2+B2, A3+B3, ... будут вычислены и использованы для построения возвращаемого массива. И для такой ситуации лучше указать ограничение количества строк/столбцов (например, согласно [`MaxDataRow`](../../cells/maxdatarow/) и [`MaxDataColumn`](../../cells/maxdatacolumn/)), иначе большой возвращаемый массив может увеличить расход памяти из‑за большого количества бесполезных данных.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Создать параметры расчёта с пользовательским движком
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Вызовите GetParamValueInArrayMode с реальными параметрами
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


