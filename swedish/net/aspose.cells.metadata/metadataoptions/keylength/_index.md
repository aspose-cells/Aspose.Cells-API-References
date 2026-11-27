---
title: "MetadataOptions.KeyLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MetadataOptions‑egenskap. Nyckellängden"
type: docs
url: /sv/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

Nyckellängden.

```csharp
public int KeyLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Skapa metadataalternativ med typ för dokumentegenskaper
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Ange krypteringsegenskaper inklusive KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Skapa metadata för en ny arbetsbok
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Lägg till anpassad egenskap
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Spara med kryptering
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Se även

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


