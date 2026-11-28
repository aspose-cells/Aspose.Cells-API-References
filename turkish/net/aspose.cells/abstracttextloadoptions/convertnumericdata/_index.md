---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractTextLoadOptions özelliği. Metin dosyasındaki dize verisinin sayısal verilere dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan değer true'tur."
type: docs
url: /tr/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Metin dosyasındaki dizeyi sayısal veriye dönüştürüp dönüştürmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur.

```csharp
public bool ConvertNumericData { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Sayısal ve dize değerleri içeren örnek CSV verisi oluşturun
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // ConvertNumericData true olarak ayarlanmış TxtLoadOptions oluşturun
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // CSV verisini bir çalışma kitabına yükleyin
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Sayısal dönüşümü gösterin
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Dönüştürülemeyen dize değerlerini gösterin
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // ConvertNumericData true olduğunda tırnak içinde olan sayıların hâlâ dönüştürüldüğünü gösterin
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


