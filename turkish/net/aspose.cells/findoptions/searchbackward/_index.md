---
title: "FindOptions.SearchBackward"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Hücrelerde geriye doğru arama yapılıp yapılmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir.

```csharp
public bool SearchBackward { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri oluşturun
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // İleriye doğru ara (varsayılan davranış)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Geriye doğru ara
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


