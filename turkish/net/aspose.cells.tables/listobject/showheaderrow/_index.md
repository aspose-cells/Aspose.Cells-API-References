---
title: "ListObject.ShowHeaderRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Bu Tablonun başlık satırını gösterip göstermediğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Bu tablonun başlık satırını gösterip göstermediğini alır ve ayarlar.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowHeaderRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı ve çalışma sayfası oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Bir liste nesnesi/tablo oluştur
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            table.ShowHeaderRow = true; // Header row is visible by default

            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Üst bilgi satırını gizle
            table.ShowHeaderRow = false;
            Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


