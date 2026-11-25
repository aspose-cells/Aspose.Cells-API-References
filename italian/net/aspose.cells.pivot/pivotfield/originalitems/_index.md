---
title: "PivotField.OriginalItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottieni gli elementi base originali"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Ottieni gli elementi base originali;

```csharp
public string[] OriginalItems { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accedi al primo campo riga
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Visualizza gli elementi originali e gli elementi raggruppati
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Salva la cartella di lavoro modificata
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


