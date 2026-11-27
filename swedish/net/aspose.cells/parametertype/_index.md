---
title: "Enum ParameterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ParameterType enum. Representerar alla parametrartyper eller returvärdestyp för funktion"
type: docs
url: /sv/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Representerar alla parametrars typ eller returvärdestyp för en funktion.

```csharp
public enum ParameterType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Skapar en arbetsbok och ett kalkylblad för att demonstrera användningen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på användning av ParameterType-enumen i en formelfunktion
            // Låt oss anta att vi definierar en anpassad funktion med specifika parametrartyper

            // Definiera en array av parametrartyper
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Exempelfunktion som använder dessa parametrartyper
            // Till exempel, att ställa in en hypotetisk anpassad funktion med definierade parametertyper
            // (Obs: Hantering av anpassade funktioner skulle bero på Aspose.Cells API:s kapacitet)

            // Spara arbetsboken för att demonstrera ändringarna
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


