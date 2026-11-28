---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Görüntü düzenleme verilerinin atılıp atılmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Görsel düzenleme verilerinin atılıp atılmadığını gösterir.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir resim ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // DiscardImageEditData'yı true olarak ayarla (varsayılan false'tur)
            workbook.Settings.DiscardImageEditData = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Ayarın uygulandığını doğrulayın
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


