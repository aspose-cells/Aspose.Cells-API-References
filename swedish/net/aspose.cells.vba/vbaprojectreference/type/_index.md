---
title: "VbaProjectReference.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReference-egenskap. Hämtar typen för denna referens"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Hämtar typen för denna referens.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Lägg till en registrerad referens till VBA-projektet
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Hämta den första referensen och demonstrera Type-egenskapen
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Spara arbetsboken
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Se även

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


