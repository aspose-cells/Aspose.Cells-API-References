---
title: "ListObject.EndColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Aralığın son sütununu alır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Aralığın son sütununu alır.

```csharp
public int EndColumn { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Bir liste nesnesi/tablo oluştur
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Orijinal son sütunu göster
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Tabloyu bir sütun daha ekleyecek şekilde yeniden boyutlandır
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Yeni son sütunu göster
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


