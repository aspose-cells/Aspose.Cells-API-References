---
title: "Style.IsFontApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını belirtin"
type: docs
url: /tr/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsFontApplied { get; set; }
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
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından bir hücreye erişin
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Hücrenin stilini al
            Style style = cell.GetStyle();
            
            // Yazı tipi ayarlarını uygulayın
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Yazı tipi uygulamasını etkinleştir
            style.IsFontApplied = true;
            
            // Değiştirilen stili hücreye geri ayarla
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


