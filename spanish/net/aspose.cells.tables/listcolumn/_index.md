---
title: "Clase ListColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.ListColumn. Representa una columna en una tabla"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Representa una columna en una Tabla.

```csharp
public class ListColumn
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Obtiene y establece la fórmula de la columna de lista. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Indica si la fórmula es una fórmula de matriz. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Obtiene y establece el nombre de la columna. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Obtiene el rango de esta columna de lista. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Obtiene y establece el tipo de cálculo en la fila Totals de la columna de lista. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Obtiene y establece las etiquetas de visualización de la fila total. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Obtiene la fórmula de esta columna de lista. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Obtiene la fórmula de la fila de totales de esta columna de lista. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Obtiene el estilo de los datos en esta columna de la tabla. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Establece la fórmula para esta columna de lista. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Obtiene la fórmula de la fila de totales de esta columna de lista. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Establece el estilo de los datos en esta columna de la tabla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

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

            // Agregar un ListObject (tabla) a la hoja de cálculo
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Acceder a la ListColumn y establecer sus propiedades
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Guarda el libro de trabajo
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


