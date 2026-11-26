---
title: "Перечисление CellValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CellValueType. Указывает тип значения ячейки"
type: docs
url: /ru/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Указывает тип значения ячейки.

```csharp
public enum CellValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| IsUnknown | `0` | Тип значения ячейки неизвестен. |
| IsNull | `1` | Пустая ячейка. Соответствующее значение должно быть null. |
| IsNumeric | `2` | Значение ячейки числовое. Соответствующее значение должно быть int или double. |
| IsDateTime | `4` | Значение ячейки — дата и время. Соответствующее значение должно быть DateTime. |
| IsString | `8` | Значение ячейки — строка. Соответствующее значение должно быть string. |
| IsBool | `16` | Значение ячейки — логическое. Соответствующее значение должно быть bool. |
| IsError | `32` | Ячейка содержит значение ошибки. Соответствующее значение должно быть строкой ошибки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Проверьте и отобразите типы значений ячеек
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Сохраните книгу
            workbook.Save("CellValueTypeExample.xlsx");
            workbook.Save("CellValueTypeExample.pdf");
        }

        private static void DisplayCellValueType(Cell cell)
        {
            Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");

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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


