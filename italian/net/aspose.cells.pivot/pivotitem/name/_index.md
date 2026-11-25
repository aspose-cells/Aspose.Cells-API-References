---
title: "PivotItem.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Ottiene il nome dell'elemento pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Ottiene il nome dell'elemento pivot.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "债券借贷";
            ws.Cells["A3"].Value = "股票";
            ws.Cells["A4"].Value = "基金";
            ws.Cells["B2"].Value = 100;
            ws.Cells["B3"].Value = 200;
            ws.Cells["B4"].Value = 300;

            // Crea tabella pivot
            int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = ws.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Accedi agli elementi pivot e dimostra la proprietà Name
            PivotField field = pivotTable.RowFields[0];
            foreach (PivotItem item in field.PivotItems)
            {
                // Nascondi tutti gli elementi tranne "债券借贷"
                item.IsHidden = item.Name != "债券借贷";
                Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
            }
            
            // Aggiorna e salva
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            wb.Save("PivotItemNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


