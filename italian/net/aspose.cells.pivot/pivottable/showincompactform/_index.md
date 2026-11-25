---
title: "PivotTable.ShowInCompactForm"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Dispone la visualizzazione della tabella pivot in forma compatta"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Disposizione della visualizzazione della tabella pivot in forma compatta.

```csharp
public void ShowInCompactForm()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dai dati di origine
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Crea un foglio di lavoro per la tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Aggiungi tabella pivot
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Imposta la tabella pivot per la visualizzazione in forma compatta
            pivotTable.ShowInCompactForm();
            
            // Calcola i dati e aggiorna
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


