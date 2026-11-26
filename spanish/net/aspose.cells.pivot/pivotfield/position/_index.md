---
title: "PivotField.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Representa el índice de PivotField en la región"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Representa el índice de [`PivotField`](../) en la región.

```csharp
public int Position { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Accede a la primera hoja de cálculo y a su tabla dinámica
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Demuestra el uso de la propiedad Position
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Utiliza position para mostrar las páginas de filtro del informe
            pt.ShowReportFilterPageByIndex(position);
            
            // Guarda el libro de trabajo
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


