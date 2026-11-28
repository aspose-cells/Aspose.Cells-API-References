---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractTextLoadOptions özelliği. Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer true'tir"
type: docs
url: /tr/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Metin dosyasındaki dizeyi tarih verisine dönüştürüp dönüştürmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Tarih dizesi içeren CSV verisi oluştur
            string csvData = "\"2023-05-15\",\"123.45\"";

            // ConvertDateTimeData false olarak ayarlanmış metin yükleme seçenekleri oluştur
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // CSV verisini yükle
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Değerleri çıktıla (dizgi olarak kalmalı)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Şimdi ConvertDateTimeData true olarak ayarlanmış şekilde yükleyin
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Dönüştürülen değerleri çıktılayın
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


