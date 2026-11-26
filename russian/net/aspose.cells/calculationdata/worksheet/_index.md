---
title: "CalculationData.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает объект Worksheet, где находится функция"
type: docs
url: /ru/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Получает объект Worksheet, где находится функция.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте некоторые данные, чтобы пример имел смысл
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Создать параметры расчёта с пользовательским движком
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Вычислить формулы с параметрами
                workbook.CalculateFormula(options);

                // Отобразить результат
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Сохранить результат
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Получить доступ к только для чтения свойству Worksheet
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


