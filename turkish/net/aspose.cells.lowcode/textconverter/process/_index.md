---
title: "TextConverter.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextConverter yöntemi. Verilen şablon dosyasını metin tabanlı dosyalar ve diğer biçimler arasında dönüştürür"
type: docs
url: /tr/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Verilen şablon dosyasını metin tabanlı dosyalar ile diğer formatlar arasında dönüştürür.

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

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // Örnek CSV dosyası oluştur
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // TextConverter örneği oluşturmadan statik Process yöntemini doğrudan çağırın
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // Geçici dosyaları temizle
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Metin tabanlı formatlar ile diğer elektronik tablo dosya formatları arasında dosya formatını dönüştürür

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
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Örnek bir metin dosyası oluşturun
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // LowCode seçenekleriyle metin dosyasını işleyin
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


