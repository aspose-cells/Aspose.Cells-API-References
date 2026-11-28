---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsLoadOptions yapıcı. ODS dosyası yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

ODS dosyasını yükleme seçeneklerini temsil eder.

```csharp
public OdsLoadOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // OdsLoadOptions'ı yapıcı kullanarak oluştur
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Hiperlink stilini Excel varsayılanlarını kullanacak şekilde ayarla
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // ODS dosyasını yükleme seçenekleriyle yükle
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // XLSX olarak kaydet
            workbook.Save("output.xlsx");
            
            // Hiperlink stilinin uygulandığını doğrula
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

ODS dosyasını yükleme seçeneklerini temsil eder.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | LoadFormat | Yükleme formatı türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Mevcut değilse örnek ODS dosyası oluştur
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // LoadFormat parametresiyle OdsLoadOptions oluştur
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Oluşturulan yükleme seçenekleriyle çalışma kitabını yükle
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Başarılı yüklemeyi göstermek için kaydet
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


