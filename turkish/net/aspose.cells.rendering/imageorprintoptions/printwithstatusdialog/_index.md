---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. PrintWithStatusDialog true ise mevcut yazdırma durumunu gösteren bir iletişim kutusu gösterilir. aksi takdirde böyle bir iletişim kutusu gösterilmez"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir. Aksi takdirde böyle bir iletişim kutusu gösterilmez.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabını başlat
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Görüntü veya yazdırma seçeneklerini ayarla
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Sheet render oluşturun
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // PDF'ye yazdır
            sheetRender.ToImage(0, "output.png");

            // Dosya oluşturulmasını bekle (basitleştirilmiş bekleme mantığı)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


