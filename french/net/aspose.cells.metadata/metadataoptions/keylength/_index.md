---
title: "MetadataOptions.KeyLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MetadataOptions. La longueur de la clé"
type: docs
url: /fr/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

La longueur de la clé.

```csharp
public int KeyLength { get; set; }
```

### Exemples

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
            // Créer des options de métadonnées avec le type de propriétés du document
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Définir les propriétés de chiffrement incluant KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Créer des métadonnées pour un nouveau classeur
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Ajouter une propriété personnalisée
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Enregistrer avec chiffrement
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Voir aussi

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


