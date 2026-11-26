---
title: "Cell.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает имя ячейки"
type: docs
url: /ru/net/aspose.cells/cell/name/
---
## Cell.Name property

Получает имя ячейки.

```csharp
public string Name { get; }
```

### Примечания

Имя ячейки включает букву столбца и номер строки. Например, имя ячейки в строке 0 и столбце 0 — A1.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте именованные диапазоны для ячеек с разными типами значений
            worksheet.Cells.CreateRange("A1").Name = "NumericCell";
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(42.5);

            worksheet.Cells.CreateRange("B1").Name = "StringCell";
            Cell cell2 = worksheet.Cells["B1"];
            cell2.PutValue("Hello World");

            worksheet.Cells.CreateRange("C1").Name = "DateTimeCell";
            Cell cell3 = worksheet.Cells["C1"];
            cell3.PutValue(DateTime.Now);

            // Отобразите информацию о ячейке, используя её свойство Name
            PrintCellInfo(cell1);
            PrintCellInfo(cell2);
            PrintCellInfo(cell3);
        }

        private static void PrintCellInfo(Cell cell)
        {
            Console.WriteLine($"Cell '{cell.Name}' has value: {cell.Value} and type: {cell.Type}");

            switch (cell.Type)
            {
                case CellValueType.IsNumeric:
                    Console.WriteLine("The cell contains a numeric value.");
                    break;
                case CellValueType.IsString:
                    Console.WriteLine("The cell contains a string value.");
                    break;
                case CellValueType.IsDateTime:
                    Console.WriteLine("The cell contains a DateTime value.");
                    break;
                case CellValueType.IsBool:
                    Console.WriteLine("The cell contains a boolean value.");
                    break;
                case CellValueType.IsNull:
                    Console.WriteLine("The cell is blank.");
                    break;
                case CellValueType.IsError:
                    Console.WriteLine("The cell contains an error value.");
                    break;
                default:
                    Console.WriteLine("The cell value type is unknown.");
                    break;
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


