---
title: "PivotFilter.GetTop10Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilter. Obtiene la configuración de los 10 principales del filtro"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Obtiene la configuración de los 10 principales del filtro.

```csharp
public Top10Filter GetTop10Value()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo y tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aplicar filtro de los 10 principales en el primer campo base (mostrar los 2 elementos principales por recuento)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Obtener el filtro aplicado y su valor de los 10 principales
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Mostrar los detalles del filtro
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


