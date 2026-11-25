---
title: "PivotField.ShowSubtotalAtTop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField property. Indica se visualizzare i subtotali in alto o in basso degli elementi"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

Indica se visualizzare i subtotali in alto o in basso degli elementi.

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Osservazioni

Funziona solo per i campi pivot nella regione delle righe quando ShowInOutlineForm è vero.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Aggiungi campo riga e configura la posizione del subtotale
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


