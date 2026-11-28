---
title: "PageSetup.IsHFAlignMargins"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Üst bilgi ve alt bilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. Bu özellik true ise sol üst bilgi ve alt bilgi sol kenar boşluğuyla, sağ üst bilgi ve alt bilgi sağ kenar boşluğuyla hizalanır. Bu seçenek varsayılan olarak etkindir"
type: docs
url: /tr/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Üst bilgi ve alt bilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. Bu özellik doğru ise, sol üst bilgi ve alt bilgi sol kenar boşluğuna, sağ üst bilgi ve alt bilgi ise sağ kenar boşluğuna hizalanır. Bu seçenek varsayılan olarak etkindir.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // IsHFAlignMargins değerini true olarak ayarla
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // IsHFAlignMargins değerini false olarak değiştir
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


