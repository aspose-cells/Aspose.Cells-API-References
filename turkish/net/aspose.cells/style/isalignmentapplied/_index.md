---
title: "Style.IsAlignmentApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını belirtin"
type: docs
url: /tr/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Açıklamalar

Yalnızca adlandırılmış stil için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // Hizalama özelliklerini ayarla
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Hizalama uygulamasını etkinleştir
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Hizalamanın uygulandığını doğrula
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


