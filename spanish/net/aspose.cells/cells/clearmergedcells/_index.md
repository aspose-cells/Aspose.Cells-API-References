---
title: "Cells.ClearMergedCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Cells method. Borra todos los rangos combinados"
type: docs
url: /es/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Borra todos los rangos combinados.

```csharp
public void ClearMergedCells()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear celdas combinadas en A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Borrar todas las celdas combinadas en la hoja de cálculo
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


