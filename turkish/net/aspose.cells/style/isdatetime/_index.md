---
title: "Style.IsDateTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Sayı biçiminin tarih biçimi olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Sayı biçiminin tarih biçimi olup olmadığını gösterir.

```csharp
public bool IsDateTime { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sayısal bir değer ayarla
            cells["A1"].PutValue(1230);
            
            // Hücrenin stilini al ve değiştir
            Style style = cells["A1"].GetStyle();
            
            // Tarih biçimine ayarla (15 yerleşik tarih biçimidir)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Özel tarih biçimi ayarla
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Değiştirilmiş stili hücreye geri uygula
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


