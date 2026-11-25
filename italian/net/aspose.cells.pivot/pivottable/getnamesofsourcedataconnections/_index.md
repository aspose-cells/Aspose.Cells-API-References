---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Ottiene i nomi delle connessioni dati di origine esterne"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Ottiene i nomi delle connessioni dati di origine esterna.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // Crea tabella pivot e ottieni il riferimento
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ottieni le connessioni ai dati di origine
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // Restituisci le informazioni di connessione
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


