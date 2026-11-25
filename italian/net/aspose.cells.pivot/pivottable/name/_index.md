---
title: "PivotTable.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene il nome della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/name/
---
## PivotTable.Name property

Restituisce il nome della PivotTable

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
    public class PivotTablePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Dimostra l'uso della proprietà Name
            Console.WriteLine("Pivot Table Name: " + pivotTable.Name);
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePropertyNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


