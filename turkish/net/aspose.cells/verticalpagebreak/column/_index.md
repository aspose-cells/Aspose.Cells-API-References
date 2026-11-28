---
title: "VerticalPageBreak.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VerticalPageBreak özelliği. Dikey sayfa kesmesinin sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Dikey sayfa sonunun sütun indeksini alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütun 4 ve 8'de dikey sayfa kesmeleri ekleyin
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Dikey sayfa kesmeleri koleksiyonunu alın
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Her dikey sayfa kesmesi hakkında bilgiyi göster
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


