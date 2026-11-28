---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions özelliği. Null değerinin göz ardı edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Null değeri yoksaymayı gösterir.

```csharp
public bool IgnoreNull { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Null değerli örnek JSON
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // IgnoreNull true olarak ayarlanmış JSON içe aktarma seçeneklerini yapılandırın
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // JSON verisini çalışma sayfasına içe aktar
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // İçe aktarılan veriyi doğrulayın (null Adres göz ardı edilmelidir)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // Çalışma kitabını kaydedin
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


