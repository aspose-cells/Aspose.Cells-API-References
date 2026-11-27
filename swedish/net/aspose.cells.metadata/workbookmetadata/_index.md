---
title: "Klass WorkbookMetadata"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metadata.WorkbookMetadata-klass. Representerar metadata"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Representerar metadata.

```csharp
public class WorkbookMetadata
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Skapa metadataobjektet. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Skapa metadataobjektet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla inbyggda dokumentegenskaper i kalkylarket. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylarket. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Hämtar alternativen för metadata. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Spara den modifierade metadata till strömmen. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Spara den modifierade metadata till filen. |

### Exempel

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
            // Skapa en MetadataOptions-instans
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Skapa en WorkbookMetadata-instans med ett filnamn och alternativ
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Lägg till en anpassad dokumentegenskap
            meta.CustomDocumentProperties.Add("test", "test");

            // Spara metadata till en ny fil
            meta.Save("WorkbookMetadataExample.xlsx");

            // Demonstrera åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Demonstrera åtkomst till anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Spara metadata till en ström
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


