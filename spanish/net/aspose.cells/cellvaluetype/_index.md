---
title: "Enum CellValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.CellValueType. Especifica un tipo de valor de celda"
type: docs
url: /es/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Especifica un tipo de valor de celda.

```csharp
public enum CellValueType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| IsUnknown | `0` | El tipo de valor de la celda es desconocido. |
| IsNull | `1` | Celda en blanco. El valor correspondiente debe ser nulo. |
| IsNumeric | `2` | El valor de la celda es numérico. El valor correspondiente debe ser int o double. |
| IsDateTime | `4` | El valor de la celda es datetime. El valor correspondiente debe ser DateTime. |
| IsString | `8` | El valor de la celda es una cadena. El valor correspondiente debe ser una cadena. |
| IsBool | `16` | El valor de la celda es booleano. El valor correspondiente debe ser bool. |
| IsError | `32` | La celda contiene un valor de error. El valor correspondiente debe ser una cadena de error. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Verificar y mostrar los tipos de valor de las celdas
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Guarda el libro de trabajo
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

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


