---
title: "PivotFilter.FilterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el tipo de filtro del filtro pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Obtiene el tipo de filtro del filtro dinámico.

```csharp
public PivotFilterType FilterType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo y tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aplicar filtro de valor (menor que 2) al primer campo base
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Recargar el libro de trabajo para verificar el filtro
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Obtener el filtro aplicado y demostrar la propiedad FilterType
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### Ver también

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


