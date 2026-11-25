---
title: "Classe WorkbookMetadata"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metadata.WorkbookMetadata classe. Rappresenta i metadati"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Rappresenta i metadati.

```csharp
public class WorkbookMetadata
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Crea l'oggetto dei metadati. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Crea l'oggetto dei metadati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento integrate del foglio elettronico. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento personalizzate del foglio elettronico. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Ottiene le opzioni dei metadati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Salva i metadati modificati nello stream. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Salva i metadati modificati nel file. |

### Esempi

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
            // Crea un'istanza di MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Crea un'istanza di WorkbookMetadata con un nome file e opzioni
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Aggiungi una proprietà documento personalizzata
            meta.CustomDocumentProperties.Add("test", "test");

            // Salva i metadati in un nuovo file
            meta.Save("WorkbookMetadataExample.xlsx");

            // Dimostra l'accesso alle proprietà documento integrate
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Dimostra l'accesso alle proprietà documento personalizzate
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Salva i metadati in uno stream
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


