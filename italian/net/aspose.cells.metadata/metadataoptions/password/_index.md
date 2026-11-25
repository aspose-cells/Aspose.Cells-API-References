---
title: "MetadataOptions.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MetadataOptions proprietà. Rappresenta la password di crittografia del file Workbook"
type: docs
url: /it/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Rappresenta la password di crittografia del file Workbook.

```csharp
public string Password { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea opzioni di metadati con protezione tramite password
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Crea una nuova cartella di lavoro e salvala prima
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Carica i metadati dal file salvato
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Aggiungi proprietà documento personalizzata
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Salva con metadati
            metadata.Save(filePath);
        }
    }
}
```

### Vedi anche

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


