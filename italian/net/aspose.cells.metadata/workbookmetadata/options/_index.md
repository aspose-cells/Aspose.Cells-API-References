---
title: "WorkbookMetadata.Options"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookMetadata. Ottiene le opzioni dei metadati"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Ottiene le opzioni dei metadati.

```csharp
public MetadataOptions Options { get; }
```

### Esempi

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
            // Crea opzioni di metadati per le proprietà del documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Crea una nuova istanza di metadati della cartella di lavoro con opzioni
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Visualizza i valori delle opzioni correnti
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Accedi alle proprietà del documento integrate
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Aggiungi proprietà di documento personalizzate
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Salva le modifiche ai metadati
            metadata.Save("output.xlsx");

            // Crea nuove opzioni per la crittografia
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


