---
title: "Klasse JsonLayoutOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Utility.JsonLayoutOptions Klasse. Stellt die Optionen des JSON-Layout-Typs dar"
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Stellt die Optionen des JSON‑Layouttyps dar.

```csharp
public class JsonLayoutOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Konstruktor zum Laden von JSON-Layout-Optionen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Verarbeitet Array als Tabelle. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Gibt an, ob die Zeichenkette in JSON in numerischen oder Datumswert konvertiert wird. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Liest und setzt das Format des Datumswerts. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Gibt an, ob der Titel ignoriert wird, wenn das Array eine Eigenschaft eines Objekts ist. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Gibt an, ob Nullwerte ignoriert werden. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Gibt an, ob der Titel ignoriert wird, wenn das Objekt eine Eigenschaft eines Objekts ist. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ignoriert Titel von Attributen |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Gibt an, ob das Schema dieses JSON beibehalten wird. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Liest und setzt das Format des numerischen Werts. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Liest und setzt den Stil des Titels. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle JsonLayoutOptions und setze Eigenschaften
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Beispieldaten für JSON
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Importiere JSON-Daten in ein Arbeitsblatt
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


