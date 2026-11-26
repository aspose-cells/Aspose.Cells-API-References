---
title: "Worksheet.PivotTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene todas las tablas dinámicas en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Obtiene todas las tablas dinámicas en esta hoja de cálculo.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de tablas dinámicas desde la hoja de cálculo
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Comprobar si hay alguna tabla dinámica
            if (pivotTables.Count > 0)
            {
                // Obtener la primera tabla dinámica
                PivotTable pivotTable = pivotTables[0];
                
                // Eliminar cualquier filtro existente
                pivotTable.PivotFilters.Clear();
                
                // Actualizar los datos de la tabla dinámica
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Guardar el libro de trabajo modificado
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


