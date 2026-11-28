---
title: "StyleFlag.VerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Dikey hizalama ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Dikey hizalama ayarı uygulanacak.

```csharp
public bool VerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Dikey hizalama ile bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Sadece dikey hizalama ve yazı tipi rengini uygulamak için stil bayrağı oluşturun
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Stil bayrağı ile stili ilk satıra uygulayın
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Etkisini görmek için hücrelere bazı metinler ayarlayın
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


