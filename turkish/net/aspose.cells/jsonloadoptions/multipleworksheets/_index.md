---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLoadOptions özelliği. Tüm alt düğümler dizi düğümleri olduğunda JsonObject nesnesinin her özelliğini ayrı bir çalışma sayfası olarak içe aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Tüm alt düğümler dizi düğümleri olduğunda JsonObject nesnesinin her özelliğinin tek bir çalışma sayfası olarak içe aktarılıp aktarılmayacağını gösterir.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // MultipleWorksheets etkinleştirilmiş JSON yükleme seçenekleri oluştur
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Belirtilen seçeneklerle JSON dosyasını çalışma kitabına yükle
            Workbook workbook = new Workbook("example.json", options);
            
            // İlk çalışma sayfasından verilere eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Yüklenen JSON'dan bazı örnek değerleri göster
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


