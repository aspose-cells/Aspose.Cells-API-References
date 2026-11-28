---
title: "PageSetup.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Sayfa ayarının ayarını kopyalar"
type: docs
url: /tr/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Sayfa ayarının ayarını kopyalar.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | PageSetup | Kaynak. |
| copyOptions | CopyOptions | Kopyalama seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // İlk çalışma sayfası için PageSetup özelliklerini ayarla
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // CopyOptions ile ilk çalışma sayfasından ikinci çalışma sayfasına PageSetup kopyala
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


