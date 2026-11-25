---
title: "VbaProjectReference.Twiddledlibid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProjectReference. Ottiene e imposta il Libid modificato del riferimento"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

Ottiene e imposta il Libid modificato del riferimento.

```csharp
public string Twiddledlibid { get; set; }
```

### Osservazioni

Solo per riferimento di controllo.

### Esempi

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

### Vedi anche

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


