---
title: "FindOptions.ConvertNumericData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Aranan dizge değerini sayısal veriye dönüştürüp dönüştürmeyeceğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool ConvertNumericData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sayısal değerleri dize olarak içeren örnek veri ekle
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // FindOptions oluştur ve ConvertNumericData'yi true olarak ayarla
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Tarih değerini bul (dize olarak depolanmış ancak arama sırasında sayısala dönüştürülür)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Sonucu çıktı olarak ver
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


