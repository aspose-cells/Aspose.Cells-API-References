---
title: "VbaProjectReference.Twiddledlibid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. يحصل على ويضبط Libid المعدل للمرجع"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

يحصل ويضبط Libid المعدل للمرجع.

```csharp
public string Twiddledlibid { get; set; }
```

### ملاحظات

فقط لإشارة التحكم.

### أمثلة

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

### انظر أيضًا

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


