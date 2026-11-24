---
title: "Enum CellValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellValueType enum. Gibt einen Zellwerttyp an"
type: docs
url: /de/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Gibt einen Zellwerttyp an.

```csharp
public enum CellValueType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| IsUnknown | `0` | Zellwerttyp ist unbekannt. |
| IsNull | `1` | Leere Zelle. Der entsprechende Wert sollte null sein. |
| IsNumeric | `2` | Zellwert ist numerisch. Der entsprechende Wert muss int oder double sein. |
| IsDateTime | `4` | Zellwert ist ein Datum/Zeitwert. Der entsprechende Wert muss DateTime sein. |
| IsString | `8` | Zellwert ist ein String. Der entsprechende Wert muss string sein. |
| IsBool | `16` | Zellwert ist ein Boolescher Wert. Der entsprechende Wert muss bool sein. |
| IsError | `32` | Zelle enthält einen Fehlerwert. Der entsprechende Wert muss ein Fehlerstring sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Überprüfe und zeige die Werttypen der Zellen an
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


