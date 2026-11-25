---
title: "PivotTable.ShowInOutlineForm"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Dispone la PivotTable in forma outline"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Disposizione della tabella pivot in forma outline.

```csharp
public void ShowInOutlineForm()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi foglio di lavoro con dati di esempio
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Aggiungi dati di esempio
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // Crea foglio di lavoro della tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Aggiungi la tabella pivot e ottieni il riferimento
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Mostra in forma outline
            pivotTable.ShowInOutlineForm();
            
            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


