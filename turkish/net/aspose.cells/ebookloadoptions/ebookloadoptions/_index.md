---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EbookLoadOptions yapıcı. E-kitap dosyasını yüklemek için bir seçenek oluşturur"
type: docs
url: /tr/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

E-kitap dosyasını yüklemek için bir seçenek oluşturur.

```csharp
public EbookLoadOptions()
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak EbookLoadOptions bir örnek oluşturun
            EbookLoadOptions options = new EbookLoadOptions();

            // Bazı temel özellikleri ayarla
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Belirtilen seçeneklerle bir e-kitap dosyası yükleyin
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Excel dosyası olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

E-kitap dosyasını yüklemek için bir seçenek oluşturur.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | LoadFormat | Yükleme biçimi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // LoadFormat parametresiyle EbookLoadOptions örneği oluşturun
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Onayı göster
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Örnek kullanım: Bu seçeneklerle bir çalışma kitabı yükleyin
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Sonucu kaydet
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


