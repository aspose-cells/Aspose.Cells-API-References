---
title: "PivotField.IsAscendSort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendSort { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortType o il metodo PivotField.SortBy(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendSortDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "B";
            sheet.Cells["A3"].Value = "C";
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B2"].Value = 150;
            sheet.Cells["B3"].Value = 300;
            sheet.Cells["B4"].Value = 200;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Configura ordinamento
            PivotField sortField = pivotTable.RowFields[0];
            sortField.IsAutoSort = true;
            sortField.IsAscendSort = false; // Demonstrate descending sort
            sortField.AutoSortField = 0; // Sort by first data field
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldIsAscendSortDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


