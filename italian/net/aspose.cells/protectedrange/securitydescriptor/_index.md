---
title: "ProtectedRange.SecurityDescriptor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRange. Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedervi"
type: docs
url: /it/net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo.

```csharp
public string SecurityDescriptor { get; set; }
```

### Esempi

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

### Vedi anche

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


