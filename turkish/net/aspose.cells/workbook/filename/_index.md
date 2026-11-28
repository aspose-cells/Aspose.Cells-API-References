---
title: "Workbook.FileName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Mevcut dosya adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Geçerli dosya adını alır ve ayarlar.

```csharp
public string FileName { get; set; }
```

### Açıklamalar

Eğer dosya akışla açıldıysa ve bazı dış formül referansları varsa, lütfen dosya adını ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Dosya adı özelliğini ayarla
            wb.FileName = "SampleWorkbook.xlsx";
            
            // İşlevselliği göstermek için bazı veriler ekle
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Çalışma kitabını kaydedin
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Dosya adını değiştirmeyi göster
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Dış bağlantı kullanımını göster
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


