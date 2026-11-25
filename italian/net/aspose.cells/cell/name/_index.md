---
title: "Cell.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il nome della cella"
type: docs
url: /it/net/aspose.cells/cell/name/
---
## Cell.Name property

Ottiene il nome della cella.

```csharp
public string Name { get; }
```

### Osservazioni

Il nome di una cella include la lettera della colonna e il numero della riga. Ad esempio, il nome di una cella nella riga 0 e colonna 0 è A1.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea intervalli denominati per celle con diversi tipi di valore
            worksheet.Cells.CreateRange("A1").Name = "NumericCell";
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(42.5);

            worksheet.Cells.CreateRange("B1").Name = "StringCell";
            Cell cell2 = worksheet.Cells["B1"];
            cell2.PutValue("Hello World");

            worksheet.Cells.CreateRange("C1").Name = "DateTimeCell";
            Cell cell3 = worksheet.Cells["C1"];
            cell3.PutValue(DateTime.Now);

            // Visualizza le informazioni della cella usando la loro proprietà Name
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

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


