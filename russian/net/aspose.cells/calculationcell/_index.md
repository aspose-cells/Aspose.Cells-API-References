---
title: "Класс CalculationCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CalculationCell. Представляет данные, относящиеся к вычислению одной ячейки, которая вычисляется"
type: docs
url: /ru/net/aspose.cells/calculationcell/
---
## CalculationCell class

Представляет данные, связанные с вычислением одной ячейки, которая вычисляется.

```csharp
public class CalculationCell
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Получает объект Cell, который вычисляется. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Получает индекс столбца ячейки. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Получает индекс строки ячейки. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Получает объект Workbook. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Получает объект Worksheet, в котором находится ячейка. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Устанавливает вычисленное значение для ячейки. |

### Примечания

Пользователь не должен изменять любые данные в Workbook во время процесса вычисления формул, иначе могут возникнуть неожиданные результаты или исключения. Поэтому все объекты, предоставляемые этим классом (например, объект Cell из [`Cell`](./cell/)), предназначены только для "read".

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Создать экземпляр CalculationCell с помощью рефлексии, так как конструктор непубличный
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Отобразить базовые свойства.
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Сохраните книгу
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


