---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLoadOptions yapıcı. Dosya yükleme seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Dosyayı yükleme seçeneklerini oluşturur.

```csharp
public JsonLoadOptions()
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Kaynak ve çıktı dizinleri
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Yapıcıyı kullanarak JsonLoadOptions oluşturun
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Seçeneklerle JSON dosyasını yükle
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Excel dosyası olarak kaydet
            workbook.Save(outputDir + "example.xlsx");

            // JsonSaveOptions ile JSON'a geri kaydet
            workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true
            });

            Console.WriteLine("JSON to Excel conversion completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


