---
title: "JsonSaveOptions.Indent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Girintiyi gösterir"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Girintiyi gösterir.

```csharp
public string Indent { get; set; }
```

### Açıklamalar

Girinti null veya boş ise, dışa aktarılan json biçimlendirilmez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Girintili JSON kaydetme seçeneklerini yapılandır
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Girintili JSON çıktısı ile kaydet
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


