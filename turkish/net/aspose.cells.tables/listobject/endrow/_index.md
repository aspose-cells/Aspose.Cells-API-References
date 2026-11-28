---
title: "ListObject.EndRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Aralığın son satırını alır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Aralığın son satırını alır.

```csharp
public int EndRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Örnek veri oluştur
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Liste nesnesi/tabloları oluştur
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // İlk EndRow değerini göster
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Tabloya yeni satır ekle
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Güncellenmiş EndRow değerini göster
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Çalışma kitabını kaydedin
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


