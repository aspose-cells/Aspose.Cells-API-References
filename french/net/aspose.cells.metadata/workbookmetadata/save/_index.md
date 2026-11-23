---
title: "WorkbookMetadata.Save"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookMetadata. Enregistre les métadonnées modifiées dans le fichier"
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Enregistre les métadonnées modifiées dans le fichier.

```csharp
public void Save(string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Créer de nouvelles métadonnées de classeur
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Ajouter des propriétés personnalisées
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Enregistrer avec un chemin de chaîne
            doc.Save("output.xlsb");
            
            // Vérifier le fichier enregistré
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Voir aussi

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Enregistre les métadonnées modifiées dans le flux.

```csharp
public void Save(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Chemin vers un classeur existant (veuillez vous assurer que le fichier existe dans le dossier d'exécution)
                string sourcePath = "Sample.xlsx";

                // Créer des MetadataOptions pour les propriétés de document
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Instancier WorkbookMetadata avec le fichier source et les options
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Accéder à la collection des propriétés du document intégrées (lecture seule).
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Enregistrer les métadonnées dans un nouveau fichier en utilisant un flux
                using (FileStream outputStream = new FileStream("MetadataOutput.xlsx",
                                                              FileMode.Create,
                                                              FileAccess.Write))
                {
                    metadata.Save(outputStream);
                }

                Console.WriteLine("Metadata saved successfully to stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during metadata Save: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


