---
title: "VbaProjectReference.RelativeLibid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "VbaProjectReference proprietà. Ottiene e imposta l'identificatore del progetto VBA di riferimento con un percorso relativo"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/relativelibid/
---
## VbaProjectReference.RelativeLibid property

Ottiene e imposta l'identificatore del progetto VBA di riferimento con un percorso relativo.

```csharp
public string RelativeLibid { get; set; }
```

### Osservazioni

Solo per riferimento di progetto.

### Esempi

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

### Vedi anche

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


