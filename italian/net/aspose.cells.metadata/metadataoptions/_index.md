---
title: "Classe MetadataOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metadata.MetadataOptions classe. Rappresenta le opzioni di caricamento dei metadati del file"
type: docs
url: /it/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Rappresenta le opzioni di caricamento dei metadati del file.

```csharp
public class MetadataOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Crea un'opzione per il caricamento dei metadati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | La lunghezza della chiave. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Ottiene e imposta il tipo dei metadati che viene caricato. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Rappresenta la password di crittografia del file Workbook. |

### Esempi

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
            // Crea un'istanza di MetadataOptions con un MetadataType specifico
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Imposta le proprietà
            options.Password = "your_password";
            options.KeyLength = 256;

            // Carica i metadati da una cartella di lavoro esistente
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Aggiungi una proprietà documento personalizzata
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Salva le modifiche ai metadati in un nuovo file
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


