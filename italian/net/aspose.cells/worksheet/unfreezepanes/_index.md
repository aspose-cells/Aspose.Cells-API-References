---
title: "Worksheet.UnFreezePanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Sblocca i riquadri nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Sblocca i riquadri nel worksheet.

```csharp
public void UnFreezePanes()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Blocca i riquadri nella cella C3 (righe 2, colonne 2 bloccate)
            worksheet.FreezePanes("C3", 2, 2);

            // Verifica che i riquadri siano congelati
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Scongela i riquadri
            worksheet.UnFreezePanes();

            // Verifica che i riquadri siano scongelati
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Salva la cartella di lavoro
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


