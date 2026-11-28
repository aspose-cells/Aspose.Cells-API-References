---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Hücre verisi sütunu aştığında tüm biçimlendirilmiş verinin gösterilip gösterilmeyeceğini belirtir. true ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. false ise veri Excel'deki gibi dışa aktarılır. Varsayılan değer false."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Sütunu taşan hücrenin tüm biçimlendirilmiş verisinin gösterilip gösterilmeyeceğini gösterir. True ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel gibi dışa aktarılır. Varsayılan değer false'tur.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve sütun genişliğini ayarlayın.
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // FormatDataIgnoreColumnWidth özelliğini gösterin.
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Etkiyi göstermek için farklı ayarlarla kaydedin.
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


