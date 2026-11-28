---
title: "Sınıf JsonLayoutOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Utility.JsonLayoutOptions sınıfı. JSON düzen tipi seçeneklerini temsil eder."
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

JSON düzen türü seçeneklerini temsil eder.

```csharp
public class JsonLayoutOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | JSON düzen seçeneklerini yüklemek için yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Diziyi tablo olarak işler. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | JSON içindeki dizeyi sayısal veya tarih değerine dönüştürüp dönüştürmeyeceğini gösterir. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Tarih değerinin biçimini alır ve ayarlar. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Dizi bir nesnenin özelliği ise başlığı yoksaymayı gösterir. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Null değeri yoksaymayı gösterir. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Nesne bir nesnenin özelliği ise başlığın göz ardı edilip edilmediğini gösterir. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Özelliklerin başlıklarını yoksayar |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Bu json'un şemasının tutulup tutulmayacağını gösterir. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Sayısal değerin biçimini alır ve ayarlar. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Başlığın stilini alır ve ayarlar. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // JsonLayoutOptions oluşturun ve özellikleri ayarlayın
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Örnek JSON verisi
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // JSON verisini çalışma sayfasına içe aktar
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


