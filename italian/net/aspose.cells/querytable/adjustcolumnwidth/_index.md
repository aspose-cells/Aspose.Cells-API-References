---
title: "QueryTable.AdjustColumnWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Restituisce o imposta AdjustColumnWidth dell'oggetto"
type: docs
url: /it/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Restituisce o imposta l'AdjustColumnWidth dell'oggetto.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con larghezze di colonna variabili
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Imposta manualmente le larghezze delle colonne
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Crea una tabella di query (simulata poiché la creazione reale richiede una fonte dati esterna)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Mostra il valore corrente di AdjustColumnWidth
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Imposta AdjustColumnWidth su true e dimostra l'effetto
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Simula l'aggiornamento della tabella di query (normalmente regolarebbe le larghezze delle colonne)
            // In uno scenario reale, ciò avverrebbe quando la tabella di query aggiorna i suoi dati
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Imposta AdjustColumnWidth su false e dimostra l'effetto
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Simula nuovamente l'aggiornamento (ora preserverebbe le larghezze originali delle colonne)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Salva la cartella di lavoro
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


