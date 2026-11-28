---
title: "Style.IsBorderApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Kenarlık biçimlendirmesinin uygulanıp uygulanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Kenarlık biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsBorderApplied { get; set; }
```

### Açıklamalar

Yalnızca adlandırılmış stil için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel bir stil oluştur
            Style style = workbook.CreateStyle();
            
            // Stile kenarlık ayarlarını uygula
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Kenarlığın uygulanıp uygulanmadığını kontrol et
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // IsBorderApplied özelliğini açıkça true olarak ayarlayın
            style.IsBorderApplied = true;
            
            // Stili bir hücreye uygula
            worksheet.Cells["A1"].SetStyle(style);
            
            // Kenarlık uygulamasını doğrulayın
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Çalışma kitabını kaydedin
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


