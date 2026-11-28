---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. HTML dosyası div etiketi içerdiğinde div etiketinin düzenini destekleyip desteklemeyeceğini gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

HTML dosyası `<div>` etiketini içerdiğinde düzenin desteklenip desteklenmeyeceğini gösterir. Varsayılan değer false'dur.

```csharp
public bool SupportDivTag { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // SupportDivTag etkinleştirilmiş HTML yükleme seçenekleri oluşturun
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Div etiketli HTML dosyasını yükleyin
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // İlk çalışma sayfasından verilere eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Hücre değeri ve stil bilgilerini çıktı olarak verin
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Excel dosyası olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


