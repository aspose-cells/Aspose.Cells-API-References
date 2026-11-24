---
title: "Klasse WorkbookMetadata"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metadata.WorkbookMetadata class. Stellt die Metadaten dar"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Stellt die Metadaten dar.

```csharp
public class WorkbookMetadata
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Erstellen Sie das Metadatenobjekt. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Erstellen Sie das Metadatenobjekt. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Ruft die Optionen der Metadaten ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Speichern Sie die modifizierten Metadaten im Stream. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Speichern Sie die modifizierten Metadaten in der Datei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // Instanz von MetadataOptions erstellen
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // WorkbookMetadata-Instanz mit Dateinamen und Optionen erstellen
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Eine benutzerdefinierte Dokumenteigenschaft hinzufügen
            meta.CustomDocumentProperties.Add("test", "test");

            // Speichern Sie die Metadaten in einer neuen Datei
            meta.Save("WorkbookMetadataExample.xlsx");

            // Demonstrieren Sie den Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Demonstrieren Sie den Zugriff auf benutzerdefinierte Dokumenteigenschaften
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Speichern Sie die Metadaten in einen Stream
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


