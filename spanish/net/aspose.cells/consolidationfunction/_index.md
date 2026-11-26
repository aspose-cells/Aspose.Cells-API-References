---
title: "Enumeración ConsolidationFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ConsolidationFunction enum. Representa la función de consolidación"
type: docs
url: /es/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Representa la función de consolidación.

```csharp
public enum ConsolidationFunction
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Sum | `0` | Representa la función Sum. |
| Count | `1` | Representa la función Count. |
| Average | `2` | Representa la función Average. |
| Max | `3` | Representa la función Max. |
| Min | `4` | Representa la función Min. |
| Product | `5` | Representa la función Product. |
| CountNums | `6` | Representa la función Count Nums. |
| StdDev | `7` | Representa la función StdDev. |
| StdDevp | `8` | Representa la función StdDevp. |
| Var | `9` | Representa la función Var. |
| Varp | `10` | Representa la función Varp. |
| DistinctCount | `11` | Representa la función Distinct Count. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Define el área de la celda para subtotal
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Aplicar subtotal con la función Sum
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Aplicar subtotal con la función Average
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Aplicar subtotal con la función Max
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Aplicar subtotal con la función Min
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Guarda el libro de trabajo
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Genere la salida de los resultados
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


