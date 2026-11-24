---
title: "Enum MetadataType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metadata.MetadataType enum. Stellt den Typ der Metadaten dar"
type: docs
url: /de/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Stellt den Typ der Metadaten dar.

```csharp
[Flags]
public enum MetadataType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Encryption | `1` | Verschlüsselt die Datei. |
| Decryption | `2` | Entschlüsselt die Datei. |
| DocumentProperties | `4` | Laden Sie die Eigenschaften der Datei. |

### Beispiele

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
            // Definieren Sie den Dateipfad
            string filePath = "MetadataTypeExample_original.xlsx";

            // Erstellen Sie MetadataOptions für DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Laden Sie die Arbeitsmappemetadaten
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Zugriff auf benutzerdefinierte Dokumenteigenschaften
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Einige integrierte Eigenschaften anzeigen
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Eine benutzerdefinierte Eigenschaft hinzufügen
            customProperties.Add("MyCustomProperty", "CustomValue");

            // In einer anderen Datei speichern
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


