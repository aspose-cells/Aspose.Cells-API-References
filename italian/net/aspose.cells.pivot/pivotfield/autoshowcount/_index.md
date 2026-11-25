---
title: "PivotField.AutoShowCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.AutoShowCount property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowCount { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.AutoShowCount o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso tra 12 mesi a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 25;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi il campo riga e imposta le proprietà AutoShow
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.AutoShowCount = 2;
            rowField.IsAutoShow = true;
            rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)

            // Calcola i dati e salva
            pivotTable.CalculateData();
            workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


