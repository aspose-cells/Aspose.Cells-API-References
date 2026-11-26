---
title: "CalculationData.Cell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает объект Cell, где находится функция"
type: docs
url: /ru/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Получает объект Cell, где находится функция.

```csharp
public Cell Cell { get; }
```

### Примечания

При вычислении формулы без привязки её к ячейке, например с помощью [`CalculateFormula`](../../worksheet/calculateformula/), формула будет вычислена так же, как если бы она была установлена в ячейку A1, поэтому оба [`CellRow`](../cellrow/) и [`CellColumn`](../cellcolumn/) равны 0. Однако ячейка A1 в листе может не быть создана. Поэтому в подобных ситуациях это свойство будет иметь значение null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
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
                options.CustomEngine = new CellDemoEngine();

                // Вычислить формулы с параметрами
                workbook.CalculateFormula(options);

                // Отобразить результат
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Сохранить результат
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Получить доступ к только для чтения свойству Cell
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

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

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


