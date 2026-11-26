---
title: "Cells.GetMergedAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene todas las celdas combinadas"
type: docs
url: /es/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Obtiene todas las celdas combinadas.

```csharp
public CellArea[] GetMergedAreas()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear algunas celdas combinadas
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Obtener todas las áreas combinadas
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Mostrar información sobre áreas combinadas
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


