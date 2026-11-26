---
title: "CalculationCell.SetCalculatedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CalculationCell. Устанавливает вычисленное значение для ячейки"
type: docs
url: /ru/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Устанавливает вычисленное значение для ячейки.

```csharp
public void SetCalculatedValue(object v)
```

### Примечания

Пользователь может установить вычисленный результат с помощью этого метода, чтобы игнорировать автоматический расчет ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
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

                // Установить вычисленное значение с помощью метода SetCalculatedValue
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Отобразить информацию о ячейке
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Сохраните книгу
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


