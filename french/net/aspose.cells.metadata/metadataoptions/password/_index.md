---
title: "MetadataOptions.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MetadataOptions. Représente le mot de passe de chiffrement du fichier classeur"
type: docs
url: /fr/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Représente le mot de passe de chiffrement du fichier du classeur.

```csharp
public string Password { get; set; }
```

### Exemples

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
            // Créer des options de métadonnées avec protection par mot de passe
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Créer un nouveau classeur et l'enregistrer d'abord
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Charger les métadonnées depuis le fichier enregistré
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Ajouter une propriété de document personnalisée
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Enregistrer avec métadonnées
            metadata.Save(filePath);
        }
    }
}
```

### Voir aussi

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


