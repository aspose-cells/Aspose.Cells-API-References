---
title: "PivotField.Ungroup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Annulla il raggruppamento del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Annulla il raggruppamento del campo pivot.

```csharp
public void Ungroup()
```

### Esempi

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
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Annulla il raggruppamento del primo campo colonna
            pivotTable.ColumnFields[0].Ungroup();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


