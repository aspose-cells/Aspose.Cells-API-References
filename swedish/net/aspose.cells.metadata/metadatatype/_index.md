---
title: "Enum MetadataType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metadata.MetadataType enum. Representerar typen av metadata"
type: docs
url: /sv/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Representerar typen av metadata.

```csharp
[Flags]
public enum MetadataType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Encryption | `1` | Krypterar filen. |
| Decryption | `2` | Dekrypterar filen. |
| DocumentProperties | `4` | Läs in egenskaperna för filen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class MetadataTypeDemo
    {
        public static void MetadataTypeExample()
        {
            // Definiera filsökvägen
            string filePath = "MetadataTypeExample_original.xlsx";

            // Skapa MetadataOptions för DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Läs in arbetsbokens metadata
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Åtkomst till anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Visa några inbyggda egenskaper
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Lägg till en anpassad egenskap
            customProperties.Add("MyCustomProperty", "CustomValue");

            // spara till en annan fil
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


