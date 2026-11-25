---
title: "Classe JsonLayoutOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Utility.JsonLayoutOptions class. Rappresenta le opzioni del tipo di layout json"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Rappresenta le opzioni del tipo di layout JSON.

```csharp
public class JsonLayoutOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Costruttore per il caricamento delle opzioni di layout JSON. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Elabora l'Array come tabella. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Indica se convertire la stringa in json in valore numerico o data. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Restituisce e imposta il formato del valore data. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Indica se ignorare il titolo se l'array è una proprietà dell'oggetto. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Indica se ignorare i valori null. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Indica se ignorare il titolo se l'oggetto è una proprietà dell'oggetto. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ignora i titoli degli attributi |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Indica se mantenere lo schema di questo JSON. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Ottiene e imposta il formato del valore numerico. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Ottiene e imposta lo stile del titolo. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea JsonLayoutOptions e imposta le proprietà
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Dati JSON di esempio
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Importa dati JSON nel foglio di lavoro
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


