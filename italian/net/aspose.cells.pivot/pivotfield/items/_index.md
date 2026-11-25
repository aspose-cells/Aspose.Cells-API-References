---
title: "PivotField.Items"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottieni tutte le etichette degli elementi pivot in questo campo"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Ottieni tutte le etichette degli elementi pivot in questo campo.

```csharp
public string[] Items { get; }
```

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Dimostra la proprietà Items
            string[] items = pivotField.Items;
            Console.WriteLine("Pivot Field Items:");
            foreach (string item in items)
            {
                Console.WriteLine(item);
            }
            
            // Imposta l'elemento della pagina corrente
            ArrayList list = new ArrayList(items);
            if (list.Contains("Apple"))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
                Console.WriteLine("Current page item set to: Apple");
            }
            
            pivotTable.CalculateData();
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


