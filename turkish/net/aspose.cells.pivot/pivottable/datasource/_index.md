---
title: "PivotTable.DataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Pivot tablonun veri kaynağını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Pivot tablonun veri kaynağını alır ve ayarlar.

```csharp
public string[] DataSource { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataSourceDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // DataSource bilgisine eriş ve göster
            string[] dataSource = pivotTable.DataSource;
            Console.WriteLine("Pivot Table Data Sources:");
            foreach (string source in dataSource)
            {
                Console.WriteLine(source);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDataSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


