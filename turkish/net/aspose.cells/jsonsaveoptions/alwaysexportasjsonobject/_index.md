---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Dosyada yalnızca bir çalışma sayfası olsa bile Excel'i her zaman nesne olarak JSON'a dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Dosyada yalnızca bir çalışma sayfası olsa bile, Excel'i her zaman nesne olarak JSON'a dışa aktarmayı gösterir.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // İlk çalışma sayfasına bazı örnek veriler ayarla
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // JSON kaydetme seçeneklerini yapılandır
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // JSON dosyasına kaydet
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Kaydedilen JSON içeriğini göster
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


