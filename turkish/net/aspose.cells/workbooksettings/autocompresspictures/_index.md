---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirtir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirtir.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // AutoCompressPictures özelliğini etkinleştir
            workbook.Settings.AutoCompressPictures = true;
            
            // Sıkıştırmayı göstermek için örnek bir resim ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Ayarı doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


