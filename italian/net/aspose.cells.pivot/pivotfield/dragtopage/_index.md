---
title: "PivotField.DragToPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se il campo specificato può essere trascinato nella regione della pagina. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi e configura DragToPage
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // Dimostra la proprietà DragToPage
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva cartella di lavoro
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


