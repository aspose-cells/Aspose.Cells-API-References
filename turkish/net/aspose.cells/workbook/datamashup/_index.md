---
title: "Workbook.DataMashup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Karışım (mashup) verisini alır"
type: docs
url: /tr/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Karışım verilerini alır.

```csharp
public DataMashup DataMashup { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Power Query'i tetiklemek için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Bir dosyaya kaydet
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // DataMashup'a erişmek için çalışma kitabını yeniden açın
            workbook = new Workbook(sourcePath);
            
            // Power Query formüllerine DataMashup özelliği aracılığıyla erişin
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Sorgular hakkında temel bilgileri çıktı olarak ver
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Eğer sorgular varsa, ilk sorgunun ayrıntılarını göster
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Yeni bir dosyaya kaydet
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


