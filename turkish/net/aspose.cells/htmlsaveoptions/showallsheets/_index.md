---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini gösterir.

```csharp
public bool ShowAllSheets { get; set; }
```

### Açıklamalar

Yalnızca [`SaveAsSingleFile`](../saveassinglefile/) True olduğunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            
            // İlk sayfaya veri ekleyin.
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // İkinci sayfa ekleyin.
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Üçüncü sayfa ekleyin.
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // ShowAllSheets özelliğini true olarak ayarlayarak tüm sayfaları dışa aktarın.
            saveOptions.ShowAllSheets = true;

            // Çalışma kitabını tüm sayfalar görünür şekilde HTML olarak kaydet
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


