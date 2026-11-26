---
title: "ProtectedRange.SecurityDescriptor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRange. El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango"
type: docs
url: /es/net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango.

```csharp
public string SecurityDescriptor { get; set; }
```

### Ejemplos

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

### Ver también

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


