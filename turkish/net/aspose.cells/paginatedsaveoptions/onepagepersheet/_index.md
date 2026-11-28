---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. OnePagePerSheet true ise bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacak ve pagesetup'ın diğer ayarları hâlâ etkili olacaktır"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. Sayfa ayarının kağıt boyutu geçersiz olacak ve sayfa ayarının diğer ayarları hâlâ geçerli olacaktır.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Her iki sayfaya da bazı örnek veriler ekleyin
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // OnePagePerSheet ile PDF kaydetme seçeneklerini ayarlayın
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


