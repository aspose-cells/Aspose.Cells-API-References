---
title: "ListObject.ApplyStyleToRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject yöntemi. Tablo stilini aralığa uygula"
type: docs
url: /tr/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Tablo stilini aralığa uygula.

```csharp
public void ApplyStyleToRange()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir liste nesnesi oluşturmak için örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bir liste nesnesi oluştur
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Liste nesnesinin aralığına stili uygula
            listObject.ApplyStyleToRange();

            // Bir hücrenin ön plan rengini kontrol ederek stilin uygulandığını doğrula
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // Liste nesnesini aralığa dönüştür ve doğrula
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


