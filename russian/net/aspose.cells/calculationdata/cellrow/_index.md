---
title: "CalculationData.CellRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает индекс строки ячейки, где находится функция"
type: docs
url: /ru/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Получает индекс строки ячейки, где находится функция.

```csharp
public int CellRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Установите параметры расчёта
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // Вычислить формулы
            workbook.CalculateFormula(opts);

            // Получить доступ к вычисленной ячейке и продемонстрировать свойство CellRow
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Продемонстрировать доступ к информации о строке из данных расчёта
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


