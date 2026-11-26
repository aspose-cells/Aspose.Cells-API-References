---
title: "PivotTable.ShowReportFilterPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Mostrar todas las páginas de filtro de informe según PivotField; el PivotField debe estar ubicado en los PageFields"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Muestra todas las páginas de filtro de informe según el PivotField, el PivotField debe estar ubicado en los PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageField | PivotField | El objeto PivotField |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("source.xlsx");
            
            // Acceder a la primera hoja de cálculo y tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Mostrar páginas de filtro de informe para cada campo de página
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


