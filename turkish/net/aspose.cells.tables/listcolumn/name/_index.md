---
title: "ListColumn.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn özelliği. Sütunun adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Sütunun adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Açıklamalar

Sütunun adı ayarlanırsa, ilgili hücrenin değeri de değişecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Bir tablo/list nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // İlk liste sütununun Name özelliğine erişin ve değiştirin
            listObject.ListColumns[0].Name = "NewID";
            
            // Adın ayarlandığını doğrulayın
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


