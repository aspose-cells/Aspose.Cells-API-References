---
title: "CellsHelper.GetCacheFolder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır.

```csharp
public static string GetCacheFolder()
```

### Dönüş Değeri

Belirtilen önbellek dosyaları klasörü. Belirtilmemişse, null dönecek ve gerektiğinde sistemin geçici yolu kullanılacaktır.

### Açıklamalar

Önbellek dosyaları genellikle bellek performansı düşünülerek bazı özellikler için kullanılır, örneğin büyük veri kümesini xls dosyasına kaydetmek veya hücre modeli için dosya önbelleğiyle bellek modunu kullanmak.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // Mevcut önbellek klasör yolu alın
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Önbellek klasör yolunu göster
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // İsteğe bağlı olarak yeni bir önbellek klasörü ayarlayın (ilgili yöntemi göstererek)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Değişikliği doğrulayın
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Orijinale geri dön (isteğe bağlı)
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


