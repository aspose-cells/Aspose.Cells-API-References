---
title: "WorkbookMetadata.Options"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookMetadata‑egenskap. Hämtar alternativen för metadata"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Hämtar alternativen för metadata.

```csharp
public MetadataOptions Options { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyOptionsDemo
    {
        public static void Run()
        {
            // Skapa metadataalternativ för dokumentegenskaper
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Skapa en ny arbetsboksmetadata‑instans med alternativ
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Visa aktuella alternativvärden
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Åtkomst till inbyggda dokumentegenskaper
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Lägg till anpassade dokumentegenskaper
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Spara metadataändringarna
            metadata.Save("output.xlsx");

            // Skapa nya alternativ för kryptering
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Se även

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


