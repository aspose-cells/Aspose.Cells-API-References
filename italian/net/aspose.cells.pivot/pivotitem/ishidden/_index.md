---
title: "PivotItem.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Ottiene e imposta se l'elemento pivot è nascosto"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Ottiene e imposta se l'elemento pivot è nascosto.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "债券借贷";
            worksheet.Cells["A3"].Value = "股票";
            worksheet.Cells["A4"].Value = "基金";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Accedi al campo pivot e agli elementi
            PivotField field = pivotTable.RowFields[0];
            
            // Imposta la proprietà IsHidden per mostrare solo "债券借贷"
            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = (item.Name != "债券借贷");
            }

            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotItemIsHiddenDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


