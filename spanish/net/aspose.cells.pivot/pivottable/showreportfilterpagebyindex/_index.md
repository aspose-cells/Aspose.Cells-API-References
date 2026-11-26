---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Muestra todas las páginas de filtro de informe según el índice de posición en los PageFields"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Muestra todas las páginas de filtro de informe según el índice de posición en los PageFields.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| posIndex | Int32 | El índice de posición en los PageFields |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Acceda a la primera hoja que contiene la tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Mostrar páginas de filtro de informe por índice (posición) del page field
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


