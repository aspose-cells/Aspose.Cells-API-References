---
title: "Top10Filter.Items"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10Filter. Ottiene e imposta il valore superiore o inferiore da utilizzare come criterio di filtro"
type: docs
url: /it/net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

Ottiene e imposta il valore superiore o inferiore da utilizzare come criterio di filtro.

```csharp
public int Items { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grapes");
            worksheet.Cells["A6"].PutValue("Mango");
            
            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Applica filtro top 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Ottieni il filtro e dimostra la proprietà Items
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            int itemsCount = filter.GetTop10Value().Items;
            
            Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
        }
    }
}
```

### Vedi anche

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


