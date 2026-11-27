---
title: "Klass JsonLayoutOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Utility.JsonLayoutOptions-klass. Representerar alternativen för json‑layout‑typen"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Representerar alternativen för JSON‑layouttyp.

```csharp
public class JsonLayoutOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Konstruktor för att ladda JSON‑layout‑alternativ. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Bearbetar array som tabell. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Anger om strängen i json ska konverteras till numeriskt eller datumvärde. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Hämtar och anger formatet för datumvärdet. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Anger om titeln ska ignoreras om array är en egenskap hos ett objekt. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Anger om null‑värde ska ignoreras. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Anger om titeln ska ignoreras om objekt är en egenskap hos ett objekt. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ignorerar titlar på attribut |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Anger om schemat för denna JSON ska behållas. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Hämtar och anger formatet för numeriskt värde. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Hämtar och sätter stilen för titeln. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa JsonLayoutOptions och sätt egenskaper
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Exempel på JSON‑data
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Importera JSON‑data till kalkylblad
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


