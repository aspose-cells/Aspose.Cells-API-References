---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool ConvertNumericData { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Sayısal ve dize değerleri içeren örnek veri tablosu oluşturun
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // İlk çalışma sayfasının hücrelerini alın
            Cells cells = workbook.Worksheets[0].Cells;

            // ConvertNumericData özelliği true olarak ayarlanmış içe aktarma seçenekleri oluşturun
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Sayısal dönüşümle verileri içe aktar
            cells.ImportData(dt, 0, 0, options);

            // Sonuçları göster
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


