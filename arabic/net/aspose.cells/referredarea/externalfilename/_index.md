---
title: "ReferredArea.ExternalFileName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. احصل على اسم الملف الخارجي إذا كانت هذه إشارة خارجية"
type: docs
url: /ar/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

احصل على اسم الملف الخارجي إذا كان هذا إشارة خارجية.

```csharp
public string ExternalFileName { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع إشارة خارجية
            Workbook wb = new Workbook();
            
            // إنشاء اسم يشير إلى مصنف خارجي
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // احصل على المنطقة المشار إليها
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // عرض خاصية ExternalFileName
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // تحقق من اسم الملف الخارجي
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


