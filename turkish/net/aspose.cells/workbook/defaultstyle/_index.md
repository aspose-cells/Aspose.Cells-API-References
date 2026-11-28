---
title: "Workbook.DefaultStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Çalışma kitabının varsayılan Style nesnesini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Varsayılan [`Style`](../../style/) nesnesini alır veya ayarlar.

```csharp
public Style DefaultStyle { get; set; }
```

### Açıklamalar

DefaultStyle özelliği, tüm Workbook için bir Style uygulamak için kullanışlıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Varsayılan stili alın ve yazı tipini değiştirin
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Değiştirilen stili varsayılan olarak geri uygulayın
            workbook.DefaultStyle = defaultStyle;
            
            // Bir çalışma sayfası oluşturun ve varsayılan stil ile bazı metinler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Çalışma kitabını kaydedin
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


