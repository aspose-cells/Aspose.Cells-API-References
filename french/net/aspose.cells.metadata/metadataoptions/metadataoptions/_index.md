---
title: "MetadataOptions.MetadataOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur MetadataOptions. Crée des options de chargement des métadonnées"
type: docs
url: /fr/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Crée des options de chargement des métadonnées.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| metadataType | MetadataType | Le type de métadonnées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Appeler la méthode #ctor avec le paramètre MetadataType
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Définir des propriétés supplémentaires
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Afficher les options créées
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Utiliser les options lors du chargement des métadonnées (exemple)
                // Cela serait généralement utilisé avec LoadOptions lors de l'ouverture d'un fichier
                // Remarque : Le code original a tenté de définir MetadataOptions directement sur LoadOptions,
                // mais la classe LoadOptions ne possède pas cette propriété dans la définition fournie.
                // Nous conserverons simplement la partie création des options puisque l'utilisation avec LoadOptions
                // n'est pas possible avec la définition actuelle de l'API.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Enregistrez le classeur (bien que les options de métadonnées n'affecteraient pas ce classeur vide)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


