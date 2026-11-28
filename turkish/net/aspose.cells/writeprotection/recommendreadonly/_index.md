---
title: "WriteProtection.RecommendReadOnly"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WriteProtection özelliği. Okunması Önerilen (Read Only Recommended) seçeneğinin seçili olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Okunabilirlik önerilen seçeneğinin seçili olup olmadığını gösterir.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına eriş ve bazı örnek veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // RecommendReadOnly'ı true olarak ayarlayın
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Özelliğin ayarlandığını doğrulayın
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Çalışma kitabını kaydedin
            workbook.Save("output_recommend_readonly.xlsx");

            // Ayarların kalıcı olduğunu doğrulamak için kaydedilmiş çalışma kitabını yükleyin
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


