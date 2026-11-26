---
title: "Clase TableToRangeOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.TableToRangeOptions. Representa las opciones al convertir una tabla en rango."
type: docs
url: /es/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Representa las opciones al convertir una tabla a rango.

```csharp
public class TableToRangeOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Obtiene y establece el índice de la última fila de la tabla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableToRangeOptionsDemo
    {
        public static void TableToRangeOptionsExample()
        {
            // Crear un nuevo libro de trabajo
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
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Agregar un ListObject (tabla) a la hoja de cálculo
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Establece algunas propiedades de la tabla
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Crea una instancia de TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Convierte la tabla en un rango usando las opciones
            table.ConvertToRange(options);

            // Guarda el libro de trabajo
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


