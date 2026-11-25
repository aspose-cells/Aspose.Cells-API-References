---
title: "PivotTable.RowHeaderCaption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Ottiene e imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi foglio di lavoro dati
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Aggiungi dati di esempio
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Aggiungi foglio di lavoro della tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Aggiungi una tabella pivot e ottieni il suo indice
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Ottieni l'istanza della tabella pivot
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configura la tabella pivot
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


