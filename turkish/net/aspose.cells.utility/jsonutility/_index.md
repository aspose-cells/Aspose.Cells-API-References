---
title: "Sınıf JsonUtility"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Utility.JsonUtility class. Represents the utility class of processing json"
type: docs
url: /tr/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

JSON işleme yardımcı sınıfını temsil eder.

```csharp
public class JsonUtility
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [JsonUtility](jsonutility/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Aralığı json dosyasına dışa aktarma. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Aralığı json dosyasına dışa aktarma. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Json dizesini içe aktar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // JsonUtility'nin bir örneğini oluştur
            JsonUtility jsonUtility = new JsonUtility();

            // JsonUtility sınıfının JSON içinde tanımlı herhangi bir özelliği veya yöntemi olmadığı için,
            // bağlamsal olarak örneklemesini ve potansiyel kullanımını göstereceğiz.

            // Örnek: JsonUtility'nin bir şekilde JSON verilerini işlemek için kullanılabileceği varsayımı.
            // Not: Gerçek sınıfta mevcut olan yöntem ve özelliklere bağlı olarak gerçek kullanım değişebilir.
            // Burada, hiçbir yöntem veya özellik sağlanmadığı için sadece örneklemeyi gösteriyoruz.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Potansiyel kullanımı göstermek için ek kod
            // Örneğin, JsonUtility'nin JSON işlemek için bir yöntemi olsaydı, şöyle görünebilir:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Hiçbir yöntem sağlanmadığından, örneği burada sonlandıracağız.
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


