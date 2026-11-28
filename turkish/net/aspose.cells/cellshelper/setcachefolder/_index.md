---
title: "CellsHelper.SetCacheFolder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar"
type: docs
url: /tr/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar.

```csharp
public static void SetCacheFolder(string cache)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| önbellek | String | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |

### Açıklamalar

Önbellek dosyaları genellikle bellek performansı düşünülerek bazı özellikler için kullanılır, örneğin büyük veri kümesini xls dosyasına kaydetmek veya hücre modeli için dosya önbelleğiyle bellek modunu kullanmak.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Önbellek için geçici bir dizin oluşturun
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // CellsHelper kullanarak önbellek klasörünü ayarlayın
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Önbellek klasörünün ayarlandığını doğrulayın
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // İşlevselliği göstermek için basit bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Çalışma kitabını kaydedin
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


