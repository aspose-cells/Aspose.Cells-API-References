---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions yapıcı. Office Open XML dosyasını kaydetmek için seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Office Open XML dosyasını kaydetme seçeneklerini oluşturur.

```csharp
public OoxmlSaveOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // OoxmlSaveOptions yapıcıyı gösterin
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // OOXML seçenekleriyle çalışma kitabını kaydedin
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Ayrıca Bakınız

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Office Open XML dosyasını kaydetme seçeneklerini oluşturur.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | SaveFormat | Dosya biçimi. Aşağıdaki türlerden biri olmalıdır: Xlsx, Xltx, Xlam, Xlsm veya Xltm; aksi takdirde kaydedilen biçim otomatik olarak Xlsx olarak ayarlanır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // SaveFormat parametresiyle OoxmlSaveOptions oluşturun
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Kaydetme seçeneklerinin bazı özelliklerini ayarlayın
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Çalışma kitabını belirtilen seçeneklerle kaydedin
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


