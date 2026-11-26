---
title: "CalculationCell.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationCell. Получает объект Worksheet, в котором находится ячейка"
type: docs
url: /ru/net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Получает объект Worksheet, в котором находится ячейка.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorksheetDemo
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

                // Отобразить значение свойства Worksheet
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Worksheet Index: " + calcCell.Worksheet.Index);
                Console.WriteLine("Worksheet Type: " + calcCell.Worksheet.Type);

                // Продемонстрировать другие связанные свойства
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Сохраните книгу
                workbook.Save("WorksheetDemo.xlsx");
                Console.WriteLine("Worksheet property demonstration completed successfully.");
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


