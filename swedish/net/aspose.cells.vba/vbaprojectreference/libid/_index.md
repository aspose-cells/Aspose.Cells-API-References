---
title: "VbaProjectReference.Libid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReference-egenskap. Hämtar och anger Libid för referensen"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Hämtar och anger Libid för referensen.

```csharp
public string Libid { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook targetWorkbook = new Workbook();
            
            // Läs in källarboken med VBA-projekt
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Rensa befintliga referenser i målet
            targetWorkbook.VbaProject.References.Clear();
            
            // Kopiera referenser från källan till målet
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Demonstrera användning av Libid-egenskapen
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Spara resultatet
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


