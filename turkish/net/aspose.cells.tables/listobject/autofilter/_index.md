---
title: "ListObject.AutoFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Bu tablonun otomatik filtresini alır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Bu tablonun otomatik filtresini alır.

```csharp
public AutoFilter AutoFilter { get; }
```

### Açıklamalar

Yalnızca [`HasAutoFilter`](../hasautofilter/) false olduğunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
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
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Bir ListObject oluştur
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Tüm verileri içerecek şekilde liste nesnesini yeniden boyutlandır
            listObject.Resize(0, 0, 4, 2, true);

            // AutoFilter işlevselliğine eriş ve göster
            if (listObject.AutoFilter != null)
            {
                // Yaş sütununda (sütun 2) filtre uygula
                listObject.AutoFilter.Filter(1, "25");
                
                // Filtrelenmiş verileri göster
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Filtreyi temizle
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


