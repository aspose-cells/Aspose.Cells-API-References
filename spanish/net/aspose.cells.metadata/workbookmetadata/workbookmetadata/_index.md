---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de WorkbookMetadata. Crear el objeto de metadatos"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Crea el objeto de metadatos.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String |  |
| opciones | MetadataOptions |  |

### Ejemplos

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

### Ver también

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Crea el objeto de metadatos.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream |  |
| opciones | MetadataOptions |  |

### Ejemplos

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
                // Crear un libro de trabajo simple en memoria
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Guardar el libro de trabajo en un flujo de memoria
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Crear MetadataOptions (usando propiedades de documento como ejemplo)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Demostrar el #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Acceder a la colección de propiedades de documento incorporada (solo lectura)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Guardar los metadatos en un archivo nuevo (opcional)
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

### Ver también

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


