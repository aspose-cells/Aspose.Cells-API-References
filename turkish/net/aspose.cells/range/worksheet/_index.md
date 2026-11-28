---
title: "Range.Worksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Bu aralığı içeren Worksheet nesnesini alır"
type: docs
url: /tr/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Bu aralığı içeren `Worksheet` nesnesini alır.

```csharp
public Worksheet Worksheet { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Adlandırılmış bir aralık oluştur
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Adlandırılmış bir aralık tanımla
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Aralığı isimle al (belirsizliği önlemek için Range'i tam nitelendir)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Worksheet özelliğinin kullanımını gösterin
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Hücreleri değiştirmek için Worksheet özelliğini kullanın
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Çalışma kitabını kaydedin
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


