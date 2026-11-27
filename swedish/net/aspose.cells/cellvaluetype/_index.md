---
title: "Enum CellValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellValueType enum. Anger en cellvärdestyp"
type: docs
url: /sv/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Anger en cellvärdestyp.

```csharp
public enum CellValueType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| IsUnknown | `0` | Cellvärdestypen är okänd. |
| IsNull | `1` | Tom cell. Tillhörande värde bör vara null. |
| IsNumeric | `2` | Cellvärdet är numeriskt. Tillhörande värde måste vara int eller double. |
| IsDateTime | `4` | Cellvärdet är datum/tid. Tillhörande värde måste vara DateTime. |
| IsString | `8` | Cellvärdet är en sträng. Tillhörande värde måste vara string. |
| IsBool | `16` | Cellvärdet är booleskt. Tillhörande värde måste vara bool. |
| IsError | `32` | Cellen innehåller felvärde. Tillhörande värde måste vara felsträng. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Kontrollera och visa värdetyperna för cellerna
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


