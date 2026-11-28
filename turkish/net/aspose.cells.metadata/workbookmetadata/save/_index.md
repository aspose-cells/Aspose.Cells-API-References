---
title: "WorkbookMetadata.Save"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookMetadata yöntemi. Değiştirilmiş meta verileri dosyaya kaydet"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Değiştirilmiş meta veriyi dosyaya kaydet.

```csharp
public void Save(string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Dosya adı. |

### Örnekler

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
            // Yeni bir çalışma kitabı meta verisi oluştur
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Özel özellikler ekle
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Dize yolu ile kaydet
            doc.Save("output.xlsb");
            
            // Kaydedilen dosyayı doğrula
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Değiştirilmiş meta veriyi akışa kaydet.

```csharp
public void Save(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Akış. |

### Örnekler

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
                // Mevcut bir çalışma kitabının yolu (dosyanın çalışma klasöründe mevcut olduğundan emin olun)
                string sourcePath = "Sample.xlsx";

                // Belge özellikleri için MetadataOptions oluştur
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Kaynak dosya ve seçeneklerle WorkbookMetadata örneği oluştur
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Yerleşik belge özellikleri koleksiyonuna eriş (yalnızca okunabilir)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Meta verileri bir akış kullanarak yeni bir dosyaya kaydet
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

### Ayrıca Bakınız

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


