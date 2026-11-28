---
title: "Workbook.StartAccessCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Veriye erişmek için önbellekleri kullanan oturumu başlatır"
type: docs
url: /tr/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Veriye erişmek için önbellekleri kullanan oturumu başlatır.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | AccessCacheOptions | veri erişim seçenekleri |

### Açıklamalar

Eğer belirtilen veri erişiminin önbelleği, çalışma sayfasındaki bazı veri modellerinin "read-only" olmasını gerektiriyorsa, bu çalışma kitabındaki her çalışma sayfasındaki ilgili veri modelleri "read-only" olarak kabul edilir ve kullanıcı bunları değiştirmemelidir. Veriye erişim tamamlandıktan sonra, [`CloseAccessCache`](../closeaccesscache/) aynı seçeneklerle çağrılmalı, tüm önbellekler temizlenmeli ve normal erişim modu geri kazanılmalıdır.

### Örnekler

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Koşullu biçimlendirme için stil ayarlayın
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Bazı gömülü görüntüler ekleyin
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Daha iyi performans için erişim önbelleğini başlat
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Hücre stillerine erişin (önbellekleme sayesinde daha hızlı olacaktır)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // İşlem tamamlandığında önbelleği kapatın
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Ayrıca Bakınız

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


