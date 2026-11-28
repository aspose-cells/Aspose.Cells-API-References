---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı boş hücreler içeren veriyi doldur
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // ExportEmptyCells false olarak ayarlanmış JsonSaveOptions oluştur
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // JSON'a kaydet - boş hücreler atlanacak
            workbook.Save("output_skip_empty.json", options);

            // ExportEmptyCells değerini true yap
            options.ExportEmptyCells = true;

            // Tekrar kaydet - boş hücreler dahil edilecek
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


