---
title: "ListColumn.Range"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn özelliği. Bu liste sütununun aralığını alır."
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Bu liste sütununun aralığını alır.

```csharp
public Range Range { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir liste nesnesi oluşturmak için örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Bir liste nesnesi oluştur
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // İlk liste sütununu alın.
            ListColumn listCol = listObj.ListColumns[0];
            
            // Liste sütununun aralığına erişin.
            Aspose.Cells.Range range = listCol.Range;
            
            // Aralık bilgilerini gösterin.
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Aralıktaki hücreleri değiştirin.
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


