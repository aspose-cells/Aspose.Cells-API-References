---
title: "WorkbookMetadata.Options"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookMetadata-Eigenschaft. Ruft die Optionen der Metadaten ab"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Ruft die Optionen der Metadaten ab.

```csharp
public MetadataOptions Options { get; }
```

### Beispiele

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
            // Erstelle Metadatenoptionen für Dokumenteigenschaften
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Erstelle eine neue WorkbookMetadata-Instanz mit Optionen
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Zeige aktuelle Optionswerte an
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Zugriff auf integrierte Dokumenteigenschaften
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Benutzerdefinierte Dokumenteigenschaften hinzufügen
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Speichere die Metadatenänderungen
            metadata.Save("output.xlsx");

            // Erstelle neue Optionen für die Verschlüsselung
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


