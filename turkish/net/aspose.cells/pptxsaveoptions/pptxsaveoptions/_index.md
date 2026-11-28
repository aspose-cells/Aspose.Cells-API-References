---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PptxSaveOptions yapıcı. pptx kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

pptx kaydetme seçeneklerini temsil eder.

```csharp
public PptxSaveOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // İkinci satırı gizle
            worksheet.Cells.Rows[1].IsHidden = true;

            // Yapıcıyı kullanarak PptxSaveOptions oluştur
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Çalışma kitabını seçeneklerle PPTX olarak kaydet
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

.pptx dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveAsImage | Boolean | True ise, çalışma kitabı .pptx dosyasının bazı resimlerine dönüştürülecek. False ise, çalışma kitabı .pptx dosyasının bazı tablolarına dönüştürülecek. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Boolean parametre ile #ctor metodunu çağır
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Ek özellikleri ayarla
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Çalışma kitabını PPTX seçenekleriyle kaydet
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


