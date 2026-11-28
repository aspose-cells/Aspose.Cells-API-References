---
title: "SpreadsheetConverter.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetConverter yöntemi. Verilen şablon dosyasını elektronik tablo dosya formatları arasında dönüştürür"
type: docs
url: /tr/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Verilen şablon dosyasını elektronik tablo dosya formatları arasında dönüştürür.

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
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Farklı elektronik tablo dosya formatları arasında dönüştürür.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Giriş dosyasıyla yükleme seçenekleri oluştur
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Çıktı dosyasıyla kaydetme seçenekleri oluştur
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Dönüştürmeyi yürüt
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


