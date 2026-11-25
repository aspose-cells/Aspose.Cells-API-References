---
title: "PivotField.DragToRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se il campo specificato può essere trascinato nella regione di riga. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToRow { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToRow. Questo metodo sarà rimosso tra 12 mesi a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Quarter";
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q3";
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;

            // Crea una tabella pivot e ottieni il suo indice
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il campo di riga e imposta la proprietà DragToRow
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToRow = true; // This allows the field to be dragged to row area

            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldDragToRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


