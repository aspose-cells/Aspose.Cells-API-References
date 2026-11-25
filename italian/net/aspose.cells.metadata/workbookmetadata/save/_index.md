---
title: "WorkbookMetadata.Save"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookMetadata. Salva i metadati modificati nel file"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Salva i metadati modificati nel file.

```csharp
public void Save(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome del file. |

### Esempi

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
            // Crea nuovi metadati della cartella di lavoro
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Aggiungi proprietà personalizzate
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Salva con percorso stringa
            doc.Save("output.xlsb");
            
            // Verifica il file salvato
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Vedi anche

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Salva i metadati modificati nello stream.

```csharp
public void Save(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream. |

### Esempi

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
                // Percorso a una cartella di lavoro esistente (assicura che il file esista nella cartella di esecuzione)
                string sourcePath = "Sample.xlsx";

                // Crea MetadataOptions per le proprietà documento
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Istanzia WorkbookMetadata con il file sorgente e le opzioni
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Accedi alla collezione delle proprietà del documento integrate (sola lettura)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Salva i metadati in un nuovo file usando uno stream
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

### Vedi anche

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


