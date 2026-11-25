---
title: "Enum MetadataType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metadata.MetadataType enum. Rappresenta il tipo di metadati"
type: docs
url: /it/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Rappresenta il tipo di metadati.

```csharp
[Flags]
public enum MetadataType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Encryption | `1` | Cifra il file. |
| Decryption | `2` | Decifra il file. |
| DocumentProperties | `4` | Carica le proprietà del file. |

### Esempi

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
            // Definisci il percorso del file
            string filePath = "MetadataTypeExample_original.xlsx";

            // Crea MetadataOptions per DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Carica i metadati del workbook
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Accedi alle proprietà personalizzate del documento
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Visualizza alcune proprietà integrate
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Aggiungi una proprietà personalizzata
            customProperties.Add("MyCustomProperty", "CustomValue");

            // salva in un file diverso
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


