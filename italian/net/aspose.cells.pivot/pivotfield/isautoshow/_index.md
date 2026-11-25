---
title: "PivotField.IsAutoShow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se il campo PivotTable specificato è mostrato automaticamente"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Indica se il campo PivotTable specificato è mostrato automaticamente.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsAutoShow property  or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoShow { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsAutoShow o il metodo PivotField.Top10AutoShow() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi un campo dati e configura IsAutoShow
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // Abilita AutoShow e configura le impostazioni
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Restituisci il valore della proprietà IsAutoShow
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


