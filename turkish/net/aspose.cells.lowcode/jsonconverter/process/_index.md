---
title: "JsonConverter.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonConverter yöntemi. Verilen şablon dosyasını json ve diğer formatlar arasında dönüştürür"
type: docs
url: /tr/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Verilen şablon dosyasını JSON ile diğer formatlar arasında dönüştürür.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | String | Dönüştürülecek şablon dosyası |
| resultFile | String | Ortaya çıkan dosya |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Örnek JSON verisi oluşturun ve geçici dosyaya yazın
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // JsonConverter'ın statik yöntemiyle dosyaları doğrudan işleyin
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Geçici JSON dosyasını temizleyin
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

JSON verisi ile diğer elektronik tablo dosya formatları arasında dönüştürür.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Örnek JSON verisi oluştur
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // JSON verisiyle bir bellek akışı oluşturun
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // LowCode seçenekleriyle JSON verisini işleyin
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


