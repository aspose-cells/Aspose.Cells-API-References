---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Gizli satır: Excel'de bu satırın yüksekliği 0'dır; HTML formatına kaydetmeden önce, eğer HtmlHiddenRowDisplayType 'Remove' ise gizli satır dışa aktarılmaz, değer 'Hidden' ise satır dışa aktarılır ancak gizli kalır. Varsayılan değer 'Hidden' dir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Gizli satır (bu satırın yüksekliği 0) Excel'de, bunu html formatına kaydetmeden önce, HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli kalır, varsayılan değer "Hidden"dır

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin ve bir satırı gizleyin.
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // HiddenRowDisplayType ile HTML kaydetme seçeneklerini ayarlayın.
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // HTML olarak kaydet
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


