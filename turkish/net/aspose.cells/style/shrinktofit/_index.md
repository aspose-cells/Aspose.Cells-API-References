---
title: "Style.ShrinkToFit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Metnin mevcut sütun genişliğine otomatik olarak sığacak şekilde küçültülüp küçültülmediğini temsil eder"
type: docs
url: /tr/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Metnin kullanılabilir sütun genişliğine sığacak şekilde otomatik olarak küçültülüp küçültülmediğini temsil eder.

```csharp
public bool ShrinkToFit { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cells koleksiyonuna eriş
            Cells cells = worksheet.Cells;
            
            // A1 hücresine sütun genişliğinden daha uzun bir metin ayarla
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Sütun genişliğini metin uzunluğundan daha küçük olacak şekilde ayarla
            cells.SetColumnWidth(0, 10);
            
            // A1 hücresinin stilini al
            Style style = cells["A1"].GetStyle();
            
            // ShrinkToFit'i true olarak ayarla
            style.ShrinkToFit = true;
            
            // Stili A1 hücresine uygula
            cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


