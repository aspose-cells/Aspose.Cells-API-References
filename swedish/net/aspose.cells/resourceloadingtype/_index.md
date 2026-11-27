---
title: "Enum ResourceLoadingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ResourceLoadingType enum. Representerar hur den länkade resursen laddas"
type: docs
url: /sv/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Representerar hur den länkade resursen laddas.

```csharp
public enum ResourceLoadingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Laddar den här resursen som vanligt. |
| Skip | `1` | Hoppar över laddning av den här resursen. |
| UserProvided | `2` | Använd ström som tillhandahålls av användaren |

### Exempel

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Spara arbetsboken till HTML med anpassad strömleverantör
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Tillhandahåll en anpassad ström för resursen
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Hoppa över att ladda resursen
                options.Stream = Stream.Null;
            }
            else
            {
                // Ladda resursen som vanligt
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Stäng strömmen om den inte är null
            options.Stream?.Close();
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


