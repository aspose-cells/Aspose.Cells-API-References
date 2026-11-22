---
title: "VbaProjectReference.RelativeLibid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. تحصل وتضبط معرف مشروع VBA المشار إليه بمسار نسبي"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/relativelibid/
---
## VbaProjectReference.RelativeLibid property

يحصل ويضبط معرف مشروع VBA المشار إليه بمسار نسبي.

```csharp
public string RelativeLibid { get; set; }
```

### ملاحظات

فقط لإشارة المشروع.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyRelativeLibidDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            VbaProject vbaProject = workbook.VbaProject;

            int referenceIndex = vbaProject.References.AddProjectRefrernce("MyReference", null, "..\\lib\\OriginalReference.xlam");
            VbaProjectReference reference = vbaProject.References[referenceIndex];

            Console.WriteLine("Current RelativeLibid value: " + reference.RelativeLibid);

            reference.RelativeLibid = "..\\new_lib\\ModifiedReference.xlam";

            Console.WriteLine("Updated RelativeLibid value: " + reference.RelativeLibid);

            workbook.Save("PropertyRelativeLibidDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


