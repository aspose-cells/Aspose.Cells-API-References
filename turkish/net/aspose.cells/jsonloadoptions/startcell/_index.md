---
title: "JsonLoadOptions.StartCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLoadOptions özelliği. Başlangıç hücresini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Başlangıç hücresini alır ve ayarlar.

```csharp
public string StartCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // StartCell özelliğiyle JSON yükleme seçenekleri oluştur
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Seçeneklerle JSON dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Örnek bir JSON dosyası oluştur
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // JSON verilerini çalışma kitabına yükle
            workbook = new Workbook("data.json", options);

            // Çalışma kitabını kaydedin
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


