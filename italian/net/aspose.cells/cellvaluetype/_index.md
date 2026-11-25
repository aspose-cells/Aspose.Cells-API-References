---
title: "Enum CellValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.CellValueType. Specifica un tipo di valore della cella"
type: docs
url: /it/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Specifica un tipo di valore della cella.

```csharp
public enum CellValueType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| IsUnknown | `0` | Il tipo di valore della cella è sconosciuto. |
| IsNull | `1` | Cella vuota. Il valore corrispondente dovrebbe essere null. |
| IsNumeric | `2` | Il valore della cella è numerico. Il valore corrispondente deve essere int o double. |
| IsDateTime | `4` | Il valore della cella è datetime. Il valore corrispondente deve essere DateTime. |
| IsString | `8` | Il valore della cella è stringa. Il valore corrispondente deve essere string. |
| IsBool | `16` | Il valore della cella è booleano. Il valore corrispondente deve essere bool. |
| IsError | `32` | La cella contiene un valore di errore. Il valore corrispondente deve essere una stringa di errore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Verifica e visualizza i tipi di valore delle celle
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


