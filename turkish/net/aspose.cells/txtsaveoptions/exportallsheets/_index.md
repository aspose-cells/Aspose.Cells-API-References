---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Tüm sayfaların metin dosyasına aktarılıp aktarılmayacağını gösterir. False ise sadece aktif sayfa, MS Excel gibi, aktarılır."
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Tüm sayfaların metin dosyasına aktarılıp aktarılmayacağını gösterir. False ise yalnızca aktif sayfa aktarılır, tıpkı MS Excel gibi.

```csharp
public bool ExportAllSheets { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // İki sayfalı bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Her iki sayfaya örnek veri ekle
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // ExportAllSheets=false (varsayılan) ile kaydedin
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // ExportAllSheets=true ile kaydedin
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


