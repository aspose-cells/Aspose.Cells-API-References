---
title: "PivotItem.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Specifica l'indice di questo elemento in tutti i PivotItem del campo"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Specificando l'indice di questo elemento in tutti i PivotItems del campo.

```csharp
public int Position { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Orange");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Dimostra la proprietà Position
            PivotField rowField = pivotTable.RowFields[0];
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
                item.Position = 0; // Set position to 0
                Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
            }

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotItemPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


