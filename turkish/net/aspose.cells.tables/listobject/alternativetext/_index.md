---
title: "ListObject.AlternativeText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Alternatif metni alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Alternatif metni alır ve ayarlar.

```csharp
public string AlternativeText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
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
            
            // Alternatif metni ve açıklamayı ayarla
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Yeniden yükle ve doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


