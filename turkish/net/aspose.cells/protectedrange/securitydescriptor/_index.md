---
title: "ProtectedRange.SecurityDescriptor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange özelliği. Güvenlik tanımlayıcısı, bu aralığı şifre girmeden düzenleyebilecek kullanıcı hesaplarını tanımlar"
type: docs
url: /tr/net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

Güvenlik tanımlayıcısı, aralığa erişmek için şifre girmeden bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar.

```csharp
public string SecurityDescriptor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertySecurityDescriptorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            ProtectedRange r = pranges[index];
            
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            r.SecurityDescriptor = securityDescriptor;
            
            string outputPath = "ProtectedRangeWithSecurityDescriptor.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with protected range security descriptor: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


