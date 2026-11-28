---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportRangeToJsonOptions özelliği. Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // B2 hücresini kasıtlı olarak boş bırak
            
            // Dışa aktarma seçeneklerini oluştur ve boş hücrelerin dışa aktarılmasını etkinleştir
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // Aralığı JSON'a dışa aktar
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


