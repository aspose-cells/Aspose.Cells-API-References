---
title: "Klass MetadataOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metadata.MetadataOptions-klass. Representerar alternativen för att läsa in metadata för filen"
type: docs
url: /sv/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Representerar alternativen för inläsning av filens metadata.

```csharp
public class MetadataOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Skapar alternativ för att läsa in metadata. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | Nyckellängden. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Hämtar och anger typen av metadata som läses in. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Anger arbetsbokens filkrypteringslösenord. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsDemo
    {
        public static void MetadataOptionsExample()
        {
            // Skapa en instans av MetadataOptions med en specifik MetadataType
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Ställ in egenskaper
            options.Password = "your_password";
            options.KeyLength = 256;

            // Läs in metadata från en befintlig arbetsbok
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Lägg till en anpassad dokumentegenskap
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Spara metadataändringarna till en ny fil
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


