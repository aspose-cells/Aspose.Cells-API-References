---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Görüntünün varsayılan çözünürlüğünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Görselin varsayılan çözünürlüğünü alır ve ayarlar.

```csharp
public int DefaultImageResolution { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Varsayılan görüntü çözünürlüğünü ayarlayın
            workbook.Settings.DefaultImageResolution = 300;
            
            // Bir çalışma sayfası ekleyin ve bir görüntü ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Varsayılan görüntü çözünürlüğünü doğrulayın
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


