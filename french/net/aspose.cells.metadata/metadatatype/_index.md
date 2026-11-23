---
title: "Énumération MetadataType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Metadata.MetadataType. Représente le type de métadonnées"
type: docs
url: /fr/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Représente le type de métadonnées.

```csharp
[Flags]
public enum MetadataType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Encryption | `1` | Crypte le fichier. |
| Decryption | `2` | Décrypte le fichier. |
| DocumentProperties | `4` | Chargez les propriétés du fichier. |

### Exemples

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
            // Définissez le chemin du fichier
            string filePath = "MetadataTypeExample_original.xlsx";

            // Créez des MetadataOptions pour les DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Chargez les métadonnées du classeur
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Accédez aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Accédez aux propriétés de document personnalisées
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Afficher certaines propriétés intégrées
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Ajoutez une propriété personnalisée
            customProperties.Add("MyCustomProperty", "CustomValue");

            // enregistrez dans un fichier différent
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


