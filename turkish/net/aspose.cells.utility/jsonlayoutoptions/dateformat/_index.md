---
title: "JsonLayoutOptions.DateFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions özelliği. Tarih değerinin biçimini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Tarih değerinin biçimini alır ve ayarlar.

```csharp
public string DateFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel tarih biçimiyle JSON içe aktarım seçeneklerini yapılandır
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // Tarih değerleriyle JSON verisini içe aktar
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // Tarihin doğru biçimlendirme ile içe aktarılıp aktarılmadığını doğrula
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


