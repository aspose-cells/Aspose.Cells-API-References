---
title: "PivotField.AutoShowField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField property. Rappresenta l'indice del campo auto show. 1 indica il PivotField stesso. Deve essere l'indice dei campi dati."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

Rappresenta l'indice del campo auto show. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.RankBy property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowField { get; set; }
```

### Osservazioni

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.RankBy o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso tra 12 mesi a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Aggiungi dati di esempio per la tabella pivot
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
            cells["B6"].Value = 10;
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Configura AutoShow per il primo campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.AutoShowCount = 2;
            pivotField.AutoShowField = 1; // Index of data field (Quantity)
            pivotField.IsAutoShow = true;
            pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
            
            // Salva la cartella di lavoro
            workbook.Save("PivotField_AutoShowField_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


