---
title: "PivotItem.GetStringValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotItem. Ottiene il valore stringa dell'elemento pivot. Se il valore è null verrà restituito"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Restituisce il valore stringa dell'elemento pivot. Se il valore è nullo, restituisce ""

```csharp
public string GetStringValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro e alla tabella pivot
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ottieni il primo campo di riga e i suoi elementi pivot
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Dimostra il metodo GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


