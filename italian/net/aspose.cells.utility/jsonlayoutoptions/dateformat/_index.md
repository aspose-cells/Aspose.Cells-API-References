---
title: "JsonLayoutOptions.DateFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Ottiene e imposta il formato del valore data"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Restituisce e imposta il formato del valore data.

```csharp
public string DateFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configura le opzioni di importazione JSON con formato data personalizzato
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // Importa dati JSON con valori di data
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // Verifica che la data sia stata importata con il formato corretto
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


