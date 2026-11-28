---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions özelliği. Diziyi tablo olarak işler"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Diziyi tablo olarak işler.

```csharp
public bool ArrayAsTable { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // JSON düzen seçeneklerini oluştur ve ArrayAsTable'i true olarak ayarla
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Örnek JSON verileri (gösterim için basitleştirilmiş)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // JSON verisini çalışma sayfasına içe aktar
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

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


