---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportRangeToJsonOptions. Indica se l'intervallo contiene una riga di intestazione"
type: docs
url: /it/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Indica se l'intervallo contiene la riga di intestazione.

```csharp
public bool HasHeaderRow { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio con intestazioni
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Crea intervallo da esportare
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Crea un'istanza di ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Mostra il valore corrente di HasHeaderRow (il valore predefinito è false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // Imposta HasHeaderRow a true
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Esporta in JSON con intestazioni
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Imposta HasHeaderRow a false
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Esporta in JSON senza intestazioni
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Salva la cartella di lavoro
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


