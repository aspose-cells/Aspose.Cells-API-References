---
title: "Font.IsBold"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Yazı tipi özelliği. Yazı tipinin kalın olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Yazı tipinin kalın olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsBold { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine eriş ve değerini ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Hücrenin stilini al ve yazı tipini kalın olarak ayarla
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Kalın özelliğini doğrula
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


