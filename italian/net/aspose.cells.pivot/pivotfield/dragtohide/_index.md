---
title: "PivotField.DragToHide"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/dragtohide/
---
## PivotField.DragToHide property

Indica se questo campo pivot può essere rimosso dalla visualizzazione PivotTable. Il valore predefinito è true.

```csharp
[Obsolete("Use PivotField.AllowRemovingFromView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToHide { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowRemovingFromView. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToHideDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;
            cells["B5"].Value = 250;

            // Crea tabella pivot - Ottieni prima l'indice, poi l'oggetto PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga e configura DragToHide
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToHide = true; // Core demonstration of the property
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldDragToHideDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


