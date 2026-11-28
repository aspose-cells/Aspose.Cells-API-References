---
title: "VerticalPageBreak.EndRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VerticalPageBreak özelliği. Dikey sayfa kesmesinin son satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Dikey sayfa sonunun bitiş satır indeksini alır.

```csharp
public int EndRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // C sütununda (indeks 2) 3 ile 8 arasındaki satırları kapsayan bir dikey sayfa kesmesi ekleyin
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // İlk dikey sayfa kesmesini alın
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Sayfa kesmesinin son satırını göster
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // EndRow yalnızca okunabilir olduğundan, onu almayı göstereceğiz ancak ayarlamayacağız
            // Aşağıdaki satır derleme hatasına neden olduğu için kaldırıldı:
            // vpb.EndRow = 10;
            
            // Bunun yerine, farklı bir son satıra sahip başka bir sayfa kesmesi ekleyeceğiz
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


