---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookMetadata yapıcı. Meta veri nesnesini oluştur"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Meta veri nesnesini oluştur.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String |  |
| seçenekler | MetadataOptions |  |

### Örnekler

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

### Ayrıca Bakınız

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Meta veri nesnesini oluştur.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream |  |
| seçenekler | MetadataOptions |  |

### Örnekler

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
                // Bellekte basit bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Çalışma kitabını bir bellek akışına kaydet
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // MetadataOptions oluştur (belge özelliklerini örnek olarak kullanarak)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- #ctor(Stream, MetadataOptions) yöntemini göster -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Yerleşik belge özellikleri koleksiyonuna eriş (yalnızca okunabilir)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Meta veriyi yeni bir dosyaya kaydet (isteğe bağlı)
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

### Ayrıca Bakınız

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


