---
title: "PivotTable.DataField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene un oggetto PivotField che rappresenta tutti i campi dati in una PivotTable. Solo lettura. Viene creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita è nella regione delle righe. Puoi trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea."
type: docs
url: /it/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Ottiene un oggetto [`PivotField`](../../pivotfield/) che rappresenta tutti i campi dati in una PivotTable. Solo lettura. Viene creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita è nella regione delle righe. Puoi trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea() .

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Osservazioni

NOTA: questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotTable.ValuesField. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Accedi e modifica le proprietà DataField
            // La posizione è solo lettura, quindi dimostreremo altre proprietà
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


