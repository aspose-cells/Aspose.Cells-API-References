---
title: "PivotField.IsAscendShow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsTop property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendShow { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsTop o il metodo PivotField.Top10AutoShow(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendShowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Imposta la proprietà IsAscendShow
            rowField.IsAscendShow = true;
            Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Imposta la proprietà IsAscendShow
            dataField.IsAscendShow = false;
            Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
            
            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


