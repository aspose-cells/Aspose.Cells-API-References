---
title: "Cell.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el nombre de la celda"
type: docs
url: /es/net/aspose.cells/cell/name/
---
## Cell.Name property

Obtiene el nombre de la celda.

```csharp
public string Name { get; }
```

### Observaciones

El nombre de una celda incluye su letra de columna y número de fila. Por ejemplo, el nombre de una celda en la fila 0 y columna 0 es A1.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear rangos con nombre para celdas con diferentes tipos de valor
            worksheet.Cells.CreateRange("A1").Name = "NumericCell";
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(42.5);

            worksheet.Cells.CreateRange("B1").Name = "StringCell";
            Cell cell2 = worksheet.Cells["B1"];
            cell2.PutValue("Hello World");

            worksheet.Cells.CreateRange("C1").Name = "DateTimeCell";
            Cell cell3 = worksheet.Cells["C1"];
            cell3.PutValue(DateTime.Now);

            // Mostrar información de la celda usando su propiedad Name
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

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


