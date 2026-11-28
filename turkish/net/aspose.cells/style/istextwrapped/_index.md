---
title: "Style.IsTextWrapped"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir hücre içindeki metnin sarılıp sarılmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Bir hücre içindeki metnin kaydırılıp kaydırılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsTextWrapped { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Hücreye uzun metin ayarlayın
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Metin sarımını etkinleştirin
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Sarılmış metni göstermek için satır yüksekliğini ayarlayın
            ws.AutoFitRow(0);
            
            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


