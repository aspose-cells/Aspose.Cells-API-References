---
title: "Style.IsPercent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Sayı biçiminin yüzde biçimi olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Sayı biçiminin yüzde biçimi olup olmadığını gösterir.

```csharp
public bool IsPercent { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine eriş ve değerini ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Hücrenin stilini al
            Style style = cell.GetStyle();
            
            // Mevcut IsPercent değerini göster
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Sayı biçimini yüzdeye ayarla (bu, IsPercent'i otomatik olarak true yapar)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // IsPercent'in artık doğru olduğunu doğrula
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Farklı formatta başka bir hücre oluştur
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Yüzde olmayan format için IsPercent'in yanlış olduğunu doğrula
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Çalışma kitabını kaydedin
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


