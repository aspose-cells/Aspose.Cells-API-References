---
title: VbaProjectReference.Twiddledlibid
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the twiddled Libid of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

Gets and sets the twiddled Libid of the reference.

```csharp
public string Twiddledlibid { get; set; }
```

### Remarks

Only for control reference.

### Examples

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

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


