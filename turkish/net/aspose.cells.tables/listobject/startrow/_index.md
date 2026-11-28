---
title: "ListObject.StartRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Aralığın başlangıç satırını alır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Aralığın başlangıç satırını alır.

```csharp
public int StartRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satır 2'den başlayarak örnek veri oluştur
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Satır 2'den başlayarak bir liste nesnesi oluştur
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // StartRow özelliğini göster
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // Başlangıç satırını "değiştirmek" için ListObject'i yeniden oluşturmalıyız
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


