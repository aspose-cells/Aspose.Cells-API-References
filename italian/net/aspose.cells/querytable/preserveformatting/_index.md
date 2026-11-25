---
title: "QueryTable.PreserveFormatting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Restituisce o imposta il PreserveFormatting dell'oggetto"
type: docs
url: /it/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Restituisce o imposta il PreserveFormatting dell'oggetto.

```csharp
public bool PreserveFormatting { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e formattazione
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Applica la formattazione all'intervallo di dati
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Applica lo stile a ogni cella nell'intervallo
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Crea una tabella di query (simulata poiché la creazione reale richiede una fonte dati esterna)
            // In un utilizzo reale, creeresti questo da una connessione esterna
            QueryTable queryTable = worksheet.QueryTables[0];

            // Visualizza il valore corrente di PreserveFormatting
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Imposta PreserveFormatting su false (non conserverà la formattazione esistente durante l'aggiornamento)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simula l'aggiornamento della query table (normalmente cancellerebbe la formattazione quando PreserveFormatting è false)
            // In uno scenario reale, ciò avverrebbe quando la tabella di query aggiorna i suoi dati
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Imposta PreserveFormatting su true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simula nuovamente l'aggiornamento (ora conserverà la formattazione)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Salva la cartella di lavoro
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


