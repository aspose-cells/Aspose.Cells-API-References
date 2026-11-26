---
title: "Enum MergedCellsShrinkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.MergedCellsShrinkType enum. Representa la estrategia para reducir celdas combinadas en operaciones como eliminar filas/columnas en blanco."
type: docs
url: /es/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Representa la estrategia para reducir celdas combinadas en operaciones como eliminar filas/columnas en blanco.

```csharp
public enum MergedCellsShrinkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Deja las celdas combinadas tal como están sin ninguna modificación. |
| ShrinkToFit | `1` | Reduce el área combinada si es necesario, eliminando filas desde la parte inferior o columnas desde la derecha, mientras asegura que todo el contenido permanezca visible. |
| KeepHeaderOnly | `2` | Solo conserva las filas/columnas de encabezado del área combinada cuando la celda superior izquierda del área combinada no está en blanco. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Inicializar datos de muestra con celdas combinadas
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Opción 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Restablecer hoja de cálculo
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Opción 2: Ninguno
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Restablecer hoja de cálculo
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Opción 3: ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


