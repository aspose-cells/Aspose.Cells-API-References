---
title: "SlicerCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SlicerCollection. Elimina il Slicer all'indice specificato"
type: docs
url: /it/net/aspose.cells.slicers/slicercollection/removeat/
---
## SlicerCollection.RemoveAt method

Elimina il Slicer all'indice specificato

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice di posizione nella collezione Slicer |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
            
            // Aggiungi alcuni dati per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aggiungi slicer
            Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
            slicers.Add(pivotTable, "Fruit", "FruitSlicer2");

            // Rimuovi il secondo slicer all'indice 1
            slicers.RemoveAt(1);
            
            // Salva la cartella di lavoro
            workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


