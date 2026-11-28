---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions yapıcı. JSON düzen seçeneklerini yükleme yapıcısı"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

JSON düzen seçeneklerini yüklemek için yapıcı.

```csharp
public JsonLayoutOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Örnek JSON verisi oluştur
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // JsonLayoutOptions'ı yapıcı kullanarak başlat
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Seçenekleri ayarla
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // JSON verisini çalışma sayfasına içe aktar
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


