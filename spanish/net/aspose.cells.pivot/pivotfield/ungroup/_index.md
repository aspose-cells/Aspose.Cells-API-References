---
title: "PivotField.Ungroup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotField. Desagrupar el campo dinámico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Desagrupar el campo dinámico.

```csharp
public void Ungroup()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Desagrupar el campo de la primera columna
            pivotTable.ColumnFields[0].Ungroup();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


