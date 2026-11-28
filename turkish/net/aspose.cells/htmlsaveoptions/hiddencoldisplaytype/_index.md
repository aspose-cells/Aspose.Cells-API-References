---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Gizli sütun: bu sütunun genişliği excel'de 0'dır. HTML formatına kaydetmeden önce, eğer HtmlHiddenColDisplayType 'Remove' ise gizli sütun çıktıya dahil edilmez; değer 'Hidden' ise sütun çıktıya dahil edilir ancak gizli kalır. Varsayılan değer 'Hidden'tır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Excel'de gizli sütun (bu sütunun genişliği 0'dır), HTML formatına kaydetmeden önce, HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli kalır, varsayılan değer "Hidden"'dır.

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // C sütununu gizle (indeks 2)
            worksheet.Cells.HideColumn(2);

            // Demonstrasyon amacıyla bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Farklı HiddenColDisplayType ayarlarıyla HTML kaydetme seçeneklerini oluşturun
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Farklı seçeneklerle kaydedin
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


