---
title: "Classe MetadataOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Metadata.MetadataOptions. Représente les options de chargement des métadonnées du fichier"
type: docs
url: /fr/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Représente les options de chargement des métadonnées du fichier.

```csharp
public class MetadataOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Crée des options de chargement des métadonnées. |

## Propriétés

| Nom | Description |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | La longueur de la clé. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Obtient et définit le type des métadonnées en cours de chargement. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Représente le mot de passe de chiffrement du fichier du classeur. |

### Exemples

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
            // Créer une instance de MetadataOptions avec un type de métadonnées spécifique
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Définir les propriétés
            options.Password = "your_password";
            options.KeyLength = 256;

            // Charger les métadonnées d'un classeur existant
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Ajouter une propriété de document personnalisée
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Enregistrer les modifications des métadonnées dans un nouveau fichier
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


