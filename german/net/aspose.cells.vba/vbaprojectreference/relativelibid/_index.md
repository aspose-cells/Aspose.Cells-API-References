---
title: "VbaProjectReference.RelativeLibid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReference-Eigenschaft. Liest und schreibt den Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/relativelibid/
---
## VbaProjectReference.RelativeLibid property

Ermittelt und setzt den Bezeichner des referenzierten VBA‑Projekts mit einem relativen Pfad.

```csharp
public string RelativeLibid { get; set; }
```

### Hinweise

Nur für Projektreferenz.

### Beispiele

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

### Siehe auch

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


