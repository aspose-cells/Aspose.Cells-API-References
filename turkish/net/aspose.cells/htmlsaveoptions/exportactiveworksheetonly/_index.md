---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Yalnızca aktif çalışma sayfasının html dosyasına aktarılıp aktarılmayacağını gösterir. Doğru ise yalnızca aktif çalışma sayfası html dosyasına aktarılır. Yanlış ise tüm çalışma kitabı html dosyasına aktarılır. Varsayılan değer yanlıştır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Yalnızca aktif çalışma sayfasının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise sadece aktif çalışma sayfası dışa aktarılır; False ise tüm çalışma kitabı dışa aktarılır. Varsayılan değer false'tur.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Her iki sayfaya örnek veri ekle
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // HTML kaydetme seçeneklerini yalnızca aktif çalışma sayfasını dışa aktarmak için ayarla
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // İlk çalışma sayfasını aktif olarak ayarla
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Yalnızca aktif çalışma sayfası ile kaydet
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Aktif sayfayı değiştir ve tekrar kaydet
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


