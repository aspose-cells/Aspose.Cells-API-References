---
title: "PivotItem.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Ottiene l'indice dell'elemento pivot nel campo cache"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Ottiene l'indice dell'elemento pivot nel campo cache.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di usare la proprietà PivotItem.Position. Questo metodo sarà rimosso 6 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Ottieni il campo di riga
            PivotField rowField = pivotTable.RowFields[0];
            
            // Accedi agli elementi pivot usando la proprietà Index
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Nascondi i dettagli dell'elemento usando la proprietà Index
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Calcola e aggiorna la tabella pivot
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


