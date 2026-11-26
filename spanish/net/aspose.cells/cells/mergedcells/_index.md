---
title: "Cells.MergedCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la colección de celdas combinadas"
type: docs
url: /es/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Obtiene la colección de celdas combinadas.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Observaciones

En esta colección, cada elemento es una estructura [`CellArea`](../../cellarea/) que representa un área de celdas combinadas.

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetMergedAreas(). Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Combinar celdas en dos rangos diferentes
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Acceder a la propiedad MergedCells (solo lectura)
            ArrayList mergedRanges = cells.MergedCells;

            // Mostrar el recuento y los rangos iniciales de celdas combinadas
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Descombinar el primer rango combinado
            cells.UnMerge(0, 0, 2, 2);

            // Mostrar el recuento y los rangos actualizados de celdas combinadas
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Guardar el resultado
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


