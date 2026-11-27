---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookMetadata‑konstruktör. Skapa metadata‑objektet"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Skapa metadataobjektet.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String |  |
| alternativ | MetadataOptions |  |

### Exempel

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

### Se även

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Skapa metadataobjektet.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström |  |
| alternativ | MetadataOptions |  |

### Exempel

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
                // Skapa en enkel arbetsbok i minnet
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Spara arbetsboken till en minnesström
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Skapa MetadataOptions (med dokumentegenskaper som exempel)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Demonstrera #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Åtkomst till den inbyggda samlingen av dokumentegenskaper (skrivskyddad)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Spara metadata till en ny fil (valfritt)
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

### Se även

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


