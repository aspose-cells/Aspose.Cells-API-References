---
title: "Cell.HtmlString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücredeki verileri ve bazı biçimleri içeren html dizesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Bu hücrede veri ve bazı biçimleri içeren html dizesini alır ve ayarlar.

```csharp
public string HtmlString { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı örneği oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cells koleksiyonuna eriş
            Cells cells = worksheet.Cells;
            
            // A1 hücresine biçimlendirilmiş HTML dizesi ayarla
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Çalışma kitabını kaydedin
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


