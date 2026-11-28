---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Dosya html'ye dışa aktarılırken boş TD öğesinin zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında html dosyasının boyutu önemli ölçüde azalır. Varsayılan değer false'tur. Html dosyasını excel'e içe aktarmak veya dosyayı html'ye kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız lütfen varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Boş TD öğesinin zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında html dosyasının boyutu önemli ölçüde azalır. Varsayılan değer false'tur. Html dosyasını excel'e içe aktarmak veya dosyayı html'ye kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız lütfen varsayılan değeri koruyun.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Boş hücrelerle örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasında bazı boş hücreler oluşturun
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 kasıtlı olarak boş bırakılmıştır
            
            // MergeEmptyTdForcely etkinleştirilmiş şekilde kaydedin
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Karşılaştırma için MergeEmptyTdForcely olmadan kaydedin
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


