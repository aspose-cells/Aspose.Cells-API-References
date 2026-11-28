---
title: "Style.IsFillApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Doldurma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsFillApplied { get; set; }
```

### Açıklamalar

Yalnızca adlandırılmış stil için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir stil oluştur
            Style style = workbook.CreateStyle();
            
            // Başlangıçta, IsFillApplied false olmalıdır
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Doldurma ayarlarını uygulayın
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Doldurma özellikleri ayarlandıktan sonra, IsFillApplied true olmalıdır
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Stili bir hücreye uygula
            worksheet.Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


