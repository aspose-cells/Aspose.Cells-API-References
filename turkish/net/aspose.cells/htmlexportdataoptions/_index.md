---
title: "Enum HtmlExportDataOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlExportDataOptions enum. HTML verisini dışa aktarma seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

HTML verilerini dışa aktarma seçeneklerini temsil eder.

```csharp
public enum HtmlExportDataOptions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Table | `1` | Yalnızca tablo bölümünü içeren dosyayı html olarak dışa aktar. |
| All | `255` | Tüm verileri html olarak dışa aktar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // HtmlSaveOptions oluşturun ve HtmlExportDataOptions ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Sadece tablo bölümünü dışa aktarmak için HtmlExportDataOptions'ı değiştirin
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Çalışma kitabını tekrar HTML formatında kaydet
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


