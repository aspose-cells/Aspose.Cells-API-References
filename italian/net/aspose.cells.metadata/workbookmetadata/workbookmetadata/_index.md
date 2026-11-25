---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore WorkbookMetadata. Crea l'oggetto dei metadati"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Crea l'oggetto dei metadati.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String |  |
| opzioni | MetadataOptions |  |

### Esempi

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

### Vedi anche

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Crea l'oggetto dei metadati.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream |  |
| opzioni | MetadataOptions |  |

### Esempi

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
                // Crea una cartella di lavoro semplice in memoria
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Salva la cartella di lavoro in un flusso di memoria
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Crea MetadataOptions (utilizzando le proprietà del documento come esempio)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Dimostra il #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Accedi alla collezione delle proprietà del documento integrate (sola lettura)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Salva i metadati in un nuovo file (opzionale)
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

### Vedi anche

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


