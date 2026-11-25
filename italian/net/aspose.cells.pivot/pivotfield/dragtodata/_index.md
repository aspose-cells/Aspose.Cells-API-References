---
title: "PivotField.DragToData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se il campo specificato può essere trascinato nella regione dei valori. Il valore predefinito è true."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToData. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi il campo di riga e configura DragToData
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Aggiungi campo colonna
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


