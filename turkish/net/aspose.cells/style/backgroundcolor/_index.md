---
title: "Style.BackgroundColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir stilin arka plan rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Bir stilin arka plan rengini alır veya ayarlar.

```csharp
public Color BackgroundColor { get; set; }
```

### Açıklamalar

Bir hücrenin rengini ayarlamak istiyorsanız, lütfen Style.ForegroundColor özelliğini kullanın. Bu özellik yalnızca hücre stil deseni none veya solid dışında olduğunda etkili olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir stil nesnesi oluşturun
            Style style = workbook.CreateStyle();
            
            // Arka plan rengini sarıya ayarlayın
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Stili A1 hücresine uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


