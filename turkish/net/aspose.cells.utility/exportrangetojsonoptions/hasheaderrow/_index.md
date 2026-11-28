---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportRangeToJsonOptions özelliği. Aralığın başlık satırı içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Aralığın başlık satırı içerip içermediğini gösterir.

```csharp
public bool HasHeaderRow { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri başlıklarla doldur
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Dışa aktarılacak aralığı oluştur
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // ExportRangeToJsonOptions örneği oluştur
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Mevcut HasHeaderRow değerini göster (varsayılan false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // HasHeaderRow değerini true olarak ayarla
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Başlıklarla JSON'a dışa aktar
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // HasHeaderRow değerini false olarak ayarla
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Başlıksız JSON'a dışa aktar
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


