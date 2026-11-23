---
title: "WorkbookMetadata.Options"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookMetadata. Obtient les options des métadonnées"
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Obtient les options des métadonnées.

```csharp
public MetadataOptions Options { get; }
```

### Exemples

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
            // Créer des options de métadonnées pour les propriétés du document.
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Créer une nouvelle instance de métadonnées de classeur avec des options
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Afficher les valeurs actuelles des options
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Accédez aux propriétés de document intégrées
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Ajouter des propriétés de document personnalisées
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Enregistrer les modifications des métadonnées
            metadata.Save("output.xlsx");

            // Créer de nouvelles options de chiffrement
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


