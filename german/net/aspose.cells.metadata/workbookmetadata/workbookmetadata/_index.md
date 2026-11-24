---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookMetadata-Konstruktor. Erstellt das Metadaten-Objekt"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Erstellen Sie das Metadatenobjekt.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String |  |
| Optionen | MetadataOptions |  |

### Beispiele

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

### Siehe auch

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Erstellen Sie das Metadatenobjekt.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream |  |
| Optionen | MetadataOptions |  |

### Beispiele

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
                // Erstelle eine einfache Arbeitsmappe im Speicher
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Speichere die Arbeitsmappe in einen Speicher-Stream
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Erstelle MetadataOptions (unter Verwendung von Dokumenteigenschaften als Beispiel)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Demonstriere den #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Greife auf die integrierte Sammlung von Dokumenteigenschaften zu (schreibgeschützt)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Speichere die Metadaten in eine neue Datei (optional)
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

### Siehe auch

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


