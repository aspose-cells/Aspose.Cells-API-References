---
title: "CalculationData.CellColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает индекс столбца ячейки, в которой находится функция"
type: docs
url: /ru/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Получает индекс столбца ячейки, где находится функция.

```csharp
public int CellColumn { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные с формулами в разных столбцах
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Создать параметры расчёта с пользовательским движком
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Вычислить формулы
                workbook.CalculateFormula(options);

                // Отобразите вычисленный результат
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Сохранить результат
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Получить доступ к только‑для‑чтения свойству CellColumn
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Продемонстрировать использование информации о столбце
                if (data.FunctionName == "SUM")
                {
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
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


