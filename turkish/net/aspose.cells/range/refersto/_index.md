---
title: "Range.RefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Başvurduğu aralıkları alır"
type: docs
url: /tr/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Aralığın referansını alır.

```csharp
public string RefersTo { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Adlandırılmış aralık için RefersTo özelliğini ayarlayın
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // İsim tarafından başvurulan aralıkları alın
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // İlk aralığın RefersTo özelliğini gösterin
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Adlandırılmış aralığı kullanan bir formül oluşturun
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Formülü hesapla
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


