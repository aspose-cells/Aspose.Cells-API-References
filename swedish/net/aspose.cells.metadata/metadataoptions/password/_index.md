---
title: "MetadataOptions.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MetadataOptions‑egenskap. Representerar lösenordet för kryptering av arbetsboksfilen"
type: docs
url: /sv/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Anger arbetsbokens filkrypteringslösenord.

```csharp
public string Password { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa metadataalternativ med lösenordsskydd
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Skapa en ny arbetsbok och spara den först
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Läs in metadata från den sparade filen
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Lägg till anpassad dokumentegenskap
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Spara med metadata
            metadata.Save(filePath);
        }
    }
}
```

### Se även

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


