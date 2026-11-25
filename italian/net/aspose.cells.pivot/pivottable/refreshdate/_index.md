---
title: "PivotTable.RefreshDate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce la data e l'ora dell'ultimo aggiornamento della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Ottiene la data e l'ora dell'ultimo aggiornamento della PivotTable.

```csharp
public DateTime RefreshDate { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Aggiorna la tabella pivot per impostare la data di aggiornamento
            pt.RefreshData();
            pt.CalculateData();

            // Visualizza le informazioni sulla data di aggiornamento
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // Salva e ricarica per dimostrare la persistenza
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Ricarica e mostra nuovamente la data di aggiornamento
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


