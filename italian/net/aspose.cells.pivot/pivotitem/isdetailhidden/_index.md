---
title: "PivotItem.IsDetailHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Ottiene e imposta se il dettaglio di questo elemento pivot è nascosto"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

Ottiene e imposta se il dettaglio di questo elemento pivot è nascosto.

```csharp
public bool IsDetailHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campi di riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Nascondi i dettagli per la categoria "Fruit"
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // Salva la cartella di lavoro
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


