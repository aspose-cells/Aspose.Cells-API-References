---
title: "Style.IsJustifyDistributed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücrelerin son satırdaki metin için iki yana yaslama veya dağıtılmış hizalamanın kullanılıp kullanılmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Hücrelerin son satırdaki metin için iki yana hizalama veya dağıtılmış hizalama kullanıp kullanmayacağını gösterir.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Açıklamalar

Bu, Doğu Asya hizalamaları için tipiktir ancak diğer bağlamlarda tipik değildir. Yalnızca dağıtılmış yatay hizalama kullanıldığında çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B3 hücresine eriş ve metnini ayarla
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Hücrenin stilini al ve IsJustifyDistributed özelliğini true olarak ayarla
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Özelliği doğrula
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


