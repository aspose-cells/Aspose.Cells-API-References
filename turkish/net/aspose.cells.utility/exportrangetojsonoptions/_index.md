---
title: "Sınıf ExportRangeToJsonOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Utility.ExportRangeToJsonOptions sınıfı. Aralığı JSON'a dışa aktarma seçeneklerini gösterir."
type: docs
url: /tr/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Aralığın JSON'a dışa aktarılması seçeneklerini gösterir.

```csharp
public class ExportRangeToJsonOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Hücrelerin metin değerini JSON'a dışa aktarır. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Aralığın başlık satırı içerip içermediğini gösterir. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Girintiyi gösterir. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Dışa aktarma seçeneklerini oluşturun
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Aralığı JSON'a dışa aktar
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // JSON'ı çıktı olarak ver
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Dosyaya kaydet (isteğe bağlı)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


