---
title: "Font.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Fontun adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/name/
---
## Font.Name property

[`Font`](../) adını alır veya ayarlar.

```csharp
public virtual string Name { get; set; }
```

### Açıklamalar

Bu özellik, fontun adını ayarlamak için kullanılırsa, [`SchemeType`](../schemetype/) None olarak güncellenecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Varsayılan çalışma sayfasına ve hücrelere eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Font özellikleriyle bir stil oluştur ve değiştir
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Name özelliğinin kullanımını göster
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Stili bir hücreye uygula
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


