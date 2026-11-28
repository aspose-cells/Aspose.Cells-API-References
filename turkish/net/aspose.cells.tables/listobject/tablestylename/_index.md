---
title: "ListObject.TableStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Tablo stil adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Tablo stil adını alır ve ayarlar.

```csharp
public string TableStyleName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
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
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bir liste nesnesi/tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Tablo stilini ayarla ve göster
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


