---
title: "Enumeración TotalsCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Tables.TotalsCalculation. Determina el tipo de cálculo en la fila Totals de la columna de lista"
type: docs
url: /es/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Determina el tipo de cálculo en la fila Totales de la columna de lista.

```csharp
public enum TotalsCalculation
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Sum | `6` | Representa el cálculo de totales de Suma. |
| Count | `2` | Representa el cálculo de totales de Conteo. |
| Average | `1` | Representa el cálculo de totales de Promedio. |
| Max | `4` | Representa el cálculo de totales de Máximo. |
| Min | `5` | Representa el cálculo de totales Min. |
| Var | `8` | Representa el cálculo de totales Var. |
| CountNums | `3` | Representa el cálculo de totales Count Nums. |
| StdDev | `7` | Representa el cálculo de totales StdDev. |
| None | `0` | Representa el cálculo de totales No. |
| Custom | `9` | Representa un cálculo personalizado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Poblar la hoja de cálculo con algunos datos
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Agregar una tabla a la hoja de cálculo
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Mostrar fila de totales
            table.ShowTotals = true;

            // Acceder a la quinta columna de la tabla
            ListColumn listColumn = table.ListColumns[4];

            // Establecer la propiedad TotalsCalculation a Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // Opcionalmente, establecer una fórmula para la columna
            listColumn.Formula = "=[A]";

            // Guarda el libro de trabajo
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


