---
title: "PivotField.ItemCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottiene il conteggio degli elementi base in questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Ottiene il conteggio degli elementi base in questo campo pivot.

```csharp
[Obsolete("Use PivotField.PivotItems.Count instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ItemCount { get; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems.Count. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["A6"].PutValue("Fruit");
            worksheet.Cells["A7"].PutValue("Vegetable");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(120);
            worksheet.Cells["B6"].PutValue(180);
            worksheet.Cells["B7"].PutValue(90);

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ottieni il campo pivot e visualizza il suo conteggio degli elementi
            PivotField pivotField = pivotTable.RowFields[0];
            Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldItemCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


