---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportRangeToJsonOptions özelliği. Hücrelerin string değerini json'a dışa aktarır"
type: docs
url: /tr/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Hücrelerin metin değerini JSON'a dışa aktarır.

```csharp
public bool ExportAsString { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücreleri farklı veri tipleriyle doldur
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // ExportRangeToJsonOptions örneği oluştur
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Mevcut ExportAsString değerini göster
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // ExportAsString olmadan dışa aktar (varsayılan davranış)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // ExportAsString değerini true olarak ayarla
            options.ExportAsString = true;

            // ExportAsString ile dışa aktar
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Çalışma kitabını kaydedin
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


