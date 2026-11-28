---
title: "JsonSaveOptions.ExportAsString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Hücrelerin string değerini json'a dışa aktarır"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Hücrelerin metin değerini JSON'a dışa aktarır.

```csharp
public bool ExportAsString { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sayısal değerlerle örnek veri oluştur
            cells["A1"].PutValue("Age");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue(30);
            cells["B2"].PutValue(95.5);

            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
            Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


