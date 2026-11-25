---
title: "PivotField.AutoSortField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Rappresenta l'indice del campo ordinato automaticamente. 1 indica lo stesso PivotField, altri valori indicano la posizione dei campi dati."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Rappresenta l'indice del campo ordinato automaticamente. -1 indica lo stesso PivotField, altri valori indicano la posizione dei campi dati.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotField.SortSetting.SortBy o il metodo PivotField.SortBy(). Questo metodo sarà rimosso tra 12 mesi a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Configura ordinamento automatico
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Calcola i dati e aggiorna
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


