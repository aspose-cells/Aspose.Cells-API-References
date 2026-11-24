---
title: "Klasse MetadataOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metadata.MetadataOptions Klasse. Stellt die Optionen zum Laden von Metadaten der Datei dar."
type: docs
url: /de/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Stellt die Optionen zum Laden von Metadaten der Datei dar.

```csharp
public class MetadataOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Erstellt Optionen zum Laden der Metadaten. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | Die Schlüssellänge. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Liest und setzt den Typ der Metadaten, die geladen werden. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |

### Beispiele

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
            // Erstellen Sie eine Instanz von MetadataOptions mit einem bestimmten MetadataType
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Eigenschaften festlegen
            options.Password = "your_password";
            options.KeyLength = 256;

            // Laden Sie Metadaten aus einer bestehenden Arbeitsmappe
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Eine benutzerdefinierte Dokumenteigenschaft hinzufügen
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Speichern Sie die Metadatenänderungen in einer neuen Datei
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


