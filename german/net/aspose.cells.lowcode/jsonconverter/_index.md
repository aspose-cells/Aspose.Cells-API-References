---
title: "Klasse JsonConverter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.JsonConverter class. Konverter für die Umwandlung zwischen JSON-Datenstrukturen und anderen Tabellenkalkulationsdateiformaten"
type: docs
url: /de/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Konverter für die Umwandlung zwischen JSON‑Datenstrukturen und anderen Tabellenkalkulationsdateiformaten.

```csharp
public class JsonConverter
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konvertiert zwischen JSON-Daten und anderen Tabellenkalkulationsdateiformaten. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Konvertiert die angegebene Vorlagendatei zwischen JSON und anderen Formaten. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Konvertieren Sie JSON zu Excel mit Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


