---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se vero, una stringa deve essere lunga al massimo 255 caratteri, quindi se la stringa supera i 255 caratteri verrà troncata. Se falso, una stringa non avrà la suddetta restrizione. Il valore predefinito è vero."
type: docs
url: /it/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se true, una stringa deve essere lunga al massimo 255 caratteri, quindi se la stringa supera i 255 caratteri verrà troncata. Se false, una stringa non avrà la suddetta restrizione. Il valore predefinito è true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Aggiungi righe di dati di esempio
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Aggiungi una tabella pivot
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configura i campi della tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Imposta la modalità di compatibilità
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


