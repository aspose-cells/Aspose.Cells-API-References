---
title: "ReferredArea.ExternalFileName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea özelliği. Bu bir dış referans ise dış dosya adını alın"
type: docs
url: /tr/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Bu bir dış referans ise dış dosya adını al.

```csharp
public string ExternalFileName { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Dış referanslı bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            
            // Dış bir çalışma kitabına başvuran bir ad oluşturun
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Başvurulan alanı alın
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // ExternalFileName özelliğini gösterin
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Dış dosya adını doğrulayın
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


