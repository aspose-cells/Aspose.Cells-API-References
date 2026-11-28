---
title: "ListObject.Comment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Tablonun yorumunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Tablonun yorumunu alır ve ayarlar.

```csharp
public string Comment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Liste nesnesi için örnek veri oluşturun
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // Bir liste nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // Comment özelliğini ayarlayın ve gösterin
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // Daha fazla veri içerecek şekilde liste nesnesinin boyutunu değiştirin
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


