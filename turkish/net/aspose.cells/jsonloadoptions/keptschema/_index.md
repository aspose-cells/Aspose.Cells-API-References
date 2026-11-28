---
title: "JsonLoadOptions.KeptSchema"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLoadOptions özelliği. Bu JSON'un şemasının korunup korunmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Bu json'un şemasının tutulup tutulmayacağını gösterir.

```csharp
public bool KeptSchema { get; set; }
```

### Açıklamalar

Bazen JSON dosyasını yükledikten sonra dosyayı JSON olarak kaydederiz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // JSON yükleme seçenekleri oluştur
            JsonLoadOptions options = new JsonLoadOptions();

            // KeptSchema özelliğinin varsayılan değerini göster
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // KeptSchema'yı true olarak ayarla
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Örnek bir JSON dosyası oluştur
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // KeptSchema etkinleştirilmiş JSON yükle
                Workbook workbook = new Workbook("sample.json", options);

                // Yüklenen çalışma kitabı hakkında bilgileri göster
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Çalışma kitabını kaydedin
                workbook.Save("KeptSchemaOutput.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


