---
title: "Klass JsonConverter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.JsonConverter-klass. Konverterare för konvertering mellan JSON‑datastruktur och andra kalkylbladsfilformat"
type: docs
url: /sv/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Konverterare för konvertering mellan JSON-datastruktur och andra kalkylbladsfilformat.

```csharp
public class JsonConverter
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konverterar mellan JSON‑data och andra kalkylbladsfilformat. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Konverterar given mallfil mellan JSON och andra format. |

### Exempel

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
                // Konvertera JSON till Excel med Aspose.Cells.LowCode.JsonConverter
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

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


