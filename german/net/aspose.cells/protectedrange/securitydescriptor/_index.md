---
title: "ProtectedRange.SecurityDescriptor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Eigenschaft. Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen"
type: docs
url: /de/net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort zur Zugriffserlangung angeben zu müssen.

```csharp
public string SecurityDescriptor { get; set; }
```

### Beispiele

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

### Siehe auch

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


