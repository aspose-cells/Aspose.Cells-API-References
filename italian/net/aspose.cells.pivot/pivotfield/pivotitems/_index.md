---
title: "PivotField.PivotItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Ottiene gli elementi pivot del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Ottiene gli elementi pivot del campo pivot

```csharp
public PivotItemCollection PivotItems { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPivotItemsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "A";
            worksheet.Cells["B4"].Value = 30;
            
            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Aggiorna i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ottieni il campo pivot e dimostra PivotItems
            PivotField field = pivotTable.RowFields[0];
            Console.WriteLine("Field Name: " + field.Name);
            Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
            
            // Visualizza tutti i nomi degli elementi pivot
            foreach (PivotItem item in field.PivotItems)
            {
                Console.WriteLine("Item Name: " + item.Name);
            }
        }
    }
}
```

### Vedi anche

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


