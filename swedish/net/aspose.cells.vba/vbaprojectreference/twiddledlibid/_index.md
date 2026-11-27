---
title: "VbaProjectReference.Twiddledlibid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReference-egenskap. Hämtar och anger den vridna Libid för referensen"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

Hämtar och anger det justerade Libid för referensen.

```csharp
public string Twiddledlibid { get; set; }
```

### Anmärkningar

Endast för kontrollreferens.

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTwiddledlibidDemo
    {
        public static void Run()
        {
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            Workbook targetWorkbook = new Workbook();
            
            targetWorkbook.VbaProject.References.Clear();
            
            foreach (VbaProjectReference refSrc in sourceWorkbook.VbaProject.References)
            {
                if (refSrc.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        refSrc.Name,
                        refSrc.Libid,
                        refSrc.Twiddledlibid,
                        refSrc.ExtendedLibid);
                }
            }
            
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


