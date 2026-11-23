---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur WorkbookMetadata. Crée l'objet de métadonnées."
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Créer l'objet de métadonnées.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String |  |
| options | MetadataOptions |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodCtorWithStringMetadataOptionsDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xls";
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);
            
            Console.WriteLine("WorkbookMetadata created successfully with document properties metadata.");
        }
    }
}
```

### Voir aussi

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Créer l'objet de métadonnées.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| options | MetadataOptions |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSharpctorWithStreamMetadataOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un classeur simple en mémoire.
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Enregistrer le classeur dans un flux mémoire.
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Créer MetadataOptions (en utilisant les propriétés du document comme exemple).
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Démontrer le #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Accéder à la collection des propriétés du document intégrées (lecture seule).
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Enregistrer les métadonnées dans un nouveau fichier (facultatif).
                    metadata.Save("MetadataFromStream.xlsx");
                }

                Console.WriteLine("WorkbookMetadata created and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during WorkbookMetadata #ctor demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


