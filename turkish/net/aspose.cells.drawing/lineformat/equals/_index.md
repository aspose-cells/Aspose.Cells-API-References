---
title: "LineFormat.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat method. Bu örneğin, belirtilen başka bir LineFormat nesnesiyle aynı değere sahip olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Bu örneğin, belirtilen başka bir [`LineFormat`](../) nesnesiyle aynı değere sahip olup olmadığını belirler.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak [`LineFormat`](../) nesnesi. |

### Dönüş Değeri

obj parametresinin değeri bu örnekle aynıysa true; aksi takdirde false. obj null ise, bu metod false döner.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir çizgi şekli ekle
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // İlk şeklin satır biçimini al
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Satır biçimlerini Equals yöntemiyle karşılaştır
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


