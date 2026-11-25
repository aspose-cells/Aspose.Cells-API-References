---
title: "PivotField.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Rappresenta l'indice di PivotField nella regione"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Rappresenta l'indice di [`PivotField`](../) nella regione.

```csharp
public int Position { get; }
```

### Esempi

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
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Accedi al primo foglio di lavoro e alla sua tabella pivot
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Dimostra l'uso della proprietà Position
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Usa position per mostrare le pagine di filtro del report
            pt.ShowReportFilterPageByIndex(position);
            
            // Salva la cartella di lavoro
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


