---
title: "ImageConverter.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageConverter yöntemi. Şablon dosyasını görüntülere dönüştürür"
type: docs
url: /tr/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Şablon dosyasını görüntülere dönüştürür.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | String | Görüntülere dönüştürülecek şablon dosyası. |
| resultFile | String | Oluşturulan görüntüler için sonuç dosyası (ad deseni). |

### Açıklamalar

Çıktı dosyaları, sayfa ve bölünme parçasının sıra numarası eklenerek belirtilen sonuç dosyasından oluşturulacaktır. Örneğin, belirtilen çıktı dosyası Image.png ise, oluşturulan görüntü dosyaları Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ... şeklinde olacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve örnek verilerle doldur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // İşleme için şablon dosyası olarak kaydet
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // (String, String) parametrelerini kullanarak şablonu görüntülere dönüştür
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Şablon dosyasını görüntülere dönüştürür

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |

### Açıklamalar

Çok sayfa destekleyen bir formatta (örneğin tiff) görüntüye dönüştürürken, belirtilen [`OutputFile`](../../lowcodesaveoptions/outputfile/) veya [`OutputStream`](../../lowcodesaveoptions/outputstream/) doğrudan sonuç görüntüsü için kullanılacaktır. Diğer görüntü türleri için, kaydetme seçeneklerinde çıktı olarak Stream belirtilmişse, tüm sonuç görüntüler aynı Stream'e kaydedilecektir. Aksi takdirde, çıktı dosyaları, kaydetme seçeneklerinin belirtilen çıktı dosyasından sayfa ve bölünme parçasının sıra numarası eklenerek oluşturulacaktır. Örneğin, belirtilen çıktı dosyası Image.png ise, oluşturulan görüntü dosyaları Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // LowCodeLoadOptions'ı bir şablon dosyasıyla başlat
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // LowCodeSaveOptions'ı çıktı diziniyle başlat
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Belirtilen parametrelerle Process yöntemini çalıştır
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Şablon dosyasını görüntülere dönüştürür

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Kayıt seçenekleri. Çıktısı ([`OutputFile`](../../lowcodesaveoptions/outputfile/) veya [`OutputStream`](../../lowcodesaveoptions/outputstream/)) "provider" parametresi tarafından belirleneceği için etkisizdir. |
| sağlayıcı | AbstractLowCodeSaveOptionsProvider | Oluşturulan görüntüleri kaydetmek için kayıt seçeneklerinin sağlayıcısı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // Örnek şablon oluştur
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Yükleme seçeneklerini başlat
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // LowCodeImageSaveOptions kullanarak kaydetme seçeneklerini yapılandır
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Statik Process yöntemini çağır
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // LowCodeImageSaveOptions'tan çözünürlük özelliklerine eriş
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


