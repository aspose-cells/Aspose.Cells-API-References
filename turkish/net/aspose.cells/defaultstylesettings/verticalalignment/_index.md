---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DefaultStyleSettings özelliği. Dikey hizalama için varsayılan değeri alır/ayarlar"
type: docs
url: /tr/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Dikey hizalama için varsayılan değeri alır/ayarlar

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Varsayılan dikey hizalamayı Alta ayarla
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Dikey hizalamanın tüm hücrelere uygulandığını doğrulayın
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


