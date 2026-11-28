---
title: "SaveOptions.CachedFileFolder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör"
type: docs
url: /tr/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

```csharp
public string CachedFileFolder { get; set; }
```

### Açıklamalar

Klasör belirtilmemişse, varsayılan değeri [`GetCacheFolder`](../../cellshelper/getcachefolder/) olur. Varsayılan değeri null veya boş ise ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken hiçbir önbellek dosyası kullanılmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Önbellek dosyası klasörüyle kaydetme seçeneklerini ayarla
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Çalışma kitabını kaydedin
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


