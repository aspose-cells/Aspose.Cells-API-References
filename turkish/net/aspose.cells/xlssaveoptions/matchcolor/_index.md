---
title: "XlsSaveOptions.MatchColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XlsSaveOptions özelliği. Standart renk paletinde 56 renk olduğu için yazı tipi renginin eşleşip eşleşmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Standart renk paletinde 56 renk olduğu için yazı tipi renginin eşleşip eşleşmeyeceğini belirtir.

```csharp
public bool MatchColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2 hücresine eriş ve belirli bir yazı tipi rengiyle bazı metinler ayarla
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Yazı tipi rengini maviye ayarla
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // MatchColor'i true olarak ayarlayarak kaydetme seçenekleri oluştur
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Çalışma kitabını seçeneklerle kaydet
            workbook.Save("output.xls", saveOptions);

            // Renk korunmuş mu diye doğrulamak için kaydedilen dosyayı yeniden yükle
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Yazı tipi renginin hâlâ mavi olduğunu doğrula
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Ayrıca Bakınız

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


