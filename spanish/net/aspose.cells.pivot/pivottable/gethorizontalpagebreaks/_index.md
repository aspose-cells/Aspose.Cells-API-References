---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Obtiene los saltos de página horizontales de esta tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Obtiene los saltos de página horizontales de esta tabla dinámica.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo fuente
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtener saltos de página horizontales
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Muestra los resultados
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


