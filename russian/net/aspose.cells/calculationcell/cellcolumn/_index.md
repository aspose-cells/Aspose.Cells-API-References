---
title: "CalculationCell.CellColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationCell. Возвращает индекс столбца ячейки"
type: docs
url: /ru/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Получает индекс столбца ячейки.

```csharp
public int CellColumn { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Вставьте некоторые данные и простую формулу
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Получить экземпляр CalculationCell через рефлексию (его конструктор непубличный)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Прочитать и отобразить значение свойства CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Дополнительная демонстрация связанных свойств (необязательно)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Сохранить Workbook (файл будет содержать добавленные данные)
                workbook.Save("CellColumnDemo.xlsx");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


