---
title: "ListObject.AlternativeDescription"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Alternatif açıklamayı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Alternatif açıklamayı alır ve ayarlar.

```csharp
public string AlternativeDescription { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
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

            // Bir liste nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Alternatif metni ve açıklamayı ayarla
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Özellikleri yeniden yükleyin ve doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


