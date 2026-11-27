---
title: "MetadataOptions.MetadataOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MetadataOptions-konstruktör. Skapar ett alternativ för att läsa in metadata"
type: docs
url: /sv/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Skapar alternativ för att läsa in metadata.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| metadataType | MetadataType | Typen av metadata. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Anropa #ctor-metoden med MetadataType-parameter
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Ange ytterligare egenskaper
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Visa de skapade alternativen
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Använd alternativen när metadata läses in (exempel)
                // Detta skulle vanligtvis användas med LoadOptions när en fil öppnas
                // Obs: Den ursprungliga koden försökte sätta MetadataOptions direkt på LoadOptions,
                // men LoadOptions-klassen har inte den här egenskapen i den angivna definitionen.
                // Vi behåller bara skapandet av alternativen eftersom användningen med LoadOptions
                // är inte möjlig med den nuvarande API-definitionen.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Spara arbetsboken (även om metadataalternativ inte skulle påverka denna tomma arbetsbok)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


