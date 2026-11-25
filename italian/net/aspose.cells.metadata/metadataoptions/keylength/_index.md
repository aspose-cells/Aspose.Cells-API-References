---
title: "MetadataOptions.KeyLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MetadataOptions proprietà. La lunghezza della chiave"
type: docs
url: /it/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

La lunghezza della chiave.

```csharp
public int KeyLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Crea opzioni di metadati con il tipo di proprietà del documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Imposta le proprietà di crittografia includendo KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Crea metadati per una nuova cartella di lavoro
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Aggiungi proprietà personalizzata
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Salva con crittografia
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Vedi anche

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


