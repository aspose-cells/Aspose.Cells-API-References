---
title: "Klass StreamProviderOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.StreamProviderOptions klass. Representerar strömalternativen"
type: docs
url: /sv/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Representerar strömalternativen.

```csharp
public class StreamProviderOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Initierar en ny instans av `StreamProviderOptions`-klassen. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Initierar en ny instans av `StreamProviderOptions`-klassen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Den anpassade sökvägen (URL) som användaren sparar i den genererade html-filen för den refererade källan. Om den inte definieras av användaren används DefaultPath. Till exempel kommer bladdata att sparas av användaren till d:/sheet001.htm, URL:en som används i huvud‑html‑filen bör vara "d:/sheet001.htm" eller någon annan giltig relativ sökväg som kan nås av huvud‑html‑filen. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Den standard sökvägen (URL) som sparas i den genererade html‑filen för den refererade källan. Till exempel, bladdata sparad i xxx_files/sheet001.htm, URL:en som används i huvud‑html‑filen bör vara som "src=\"xxx_files/sheet001.htm\"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Hämtar och anger typen av laddningsresurs. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Hämtar/anger strömmen |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Ställ in en minnesström för demonstration
            options.Stream = new MemoryStream();
            
            // Använd strömmen (exempel: spara arbetsboken till strömmen)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Demonstrera att stänga strömmen
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


