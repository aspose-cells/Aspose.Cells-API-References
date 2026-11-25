---
title: "SlicerCacheItem.Selected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SlicerCacheItem. Specifica se il SlicerCacheItem è selezionato o meno"
type: docs
url: /it/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Specifica se il [`SlicerCacheItem`](../) è selezionato o meno.

```csharp
public bool Selected { get; set; }
```

### Osservazioni

Si prega di utilizzare il metodo [`SelectItems`](../../slicer/selectitems/) invece se si desidera selezionare l'elemento. Poiché questa operazione di aggiornamento causa scarse prestazioni a causa del ricaricamento completo dei dati ogni volta che la selezione cambia.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Aggiungi slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Accedi agli elementi della cache slicer
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // Seleziona il primo elemento, deseleziona gli altri
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


