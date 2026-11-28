---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions yapıcı. JSON dosyası kaydetmek için seçenekler oluşturur"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

JSON dosyasını kaydetmek için seçenekler oluşturur.

```csharp
public JsonSaveOptions()
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // JSON olarak dışa aktarılacak örnek veri
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Yapıcıyı kullanarak JsonSaveOptions başlat
            JsonSaveOptions options = new JsonSaveOptions();
            
            // JSON dışa aktarma seçeneklerini ayarla
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Çalışma kitabını JSON seçenekleriyle kaydet
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


