---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Eğer AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği yalnızca bir sayfaya çıktılanır. Sayfa ayarı (pagesetup) kağıt boyutu genişliği geçersiz olur ve pagesetup'ın diğer ayarları hâlâ etkili olur"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt genişliği geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı verileri doldurun
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Görüntü kaydetme seçenekleri oluşturun
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // Çalışma kitabını bellek akışına PNG olarak kaydet
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


