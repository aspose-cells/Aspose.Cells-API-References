---
title: "WorkbookMetadata.Save"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookMetadata-Methode. Speichern Sie die geänderten Metadaten in die Datei"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Speichern Sie die modifizierten Metadaten in der Datei.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname. |

### Beispiele

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
            // Erstellen Sie neue Arbeitsmappen-Metadaten
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Benutzerdefinierte Eigenschaften hinzufügen.
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Speichern mit string-Pfad
            doc.Save("output.xlsb");
            
            // Überprüfen Sie die gespeicherte Datei
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Siehe auch

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Speichern Sie die modifizierten Metadaten im Stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Stream. |

### Beispiele

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
                // Pfad zu einer vorhandenen Arbeitsmappe (stellen Sie sicher, dass die Datei im Ausführungsordner existiert)
                string sourcePath = "Sample.xlsx";

                // Erstellen Sie MetadataOptions für Dokumenteigenschaften
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Instanziieren Sie WorkbookMetadata mit der Quelldatei und den Optionen
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Greife auf die integrierte Sammlung von Dokumenteigenschaften zu (schreibgeschützt)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Speichern Sie die Metadaten in einer neuen Datei mithilfe eines Streams
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

### Siehe auch

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


