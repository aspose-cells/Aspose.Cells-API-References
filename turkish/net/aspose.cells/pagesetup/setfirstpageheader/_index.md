---
title: "PageSetup.SetFirstPageHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının ilk sayfa üstbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffFirst true olduğunda Excel 2007'de etkilidir"
type: docs
url: /tr/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Excel dosyasının ilk sayfa üstbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffFirst doğru olduğunda Excel 2007'de etkilidir.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | String | Başlık biçimlendirme betiği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Bölüm numarası ve üstbilgi metni ile ilk sayfa üstbilgisini ayarlayın
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


