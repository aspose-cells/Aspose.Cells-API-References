---
title: "CalculationCell.Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationCell. Получает объект Workbook"
type: docs
url: /ru/net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Получает объект Workbook.

```csharp
public Workbook Workbook { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorkbookDemo
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

                // Отобразить значение свойства Workbook
                Console.WriteLine("Workbook Name: " + calcCell.Workbook.FileName);
                Console.WriteLine("Workbook Has Macro: " + calcCell.Workbook.HasMacro);
                Console.WriteLine("Workbook Worksheet Count: " + calcCell.Workbook.Worksheets.Count);

                // Продемонстрировать связанные свойства для контекста
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Сохраните книгу
                workbook.Save("WorkbookDemo.xlsx");
                Console.WriteLine("Workbook property demonstration completed successfully.");
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

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


