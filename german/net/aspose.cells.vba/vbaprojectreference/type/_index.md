---
title: "VbaProjectReference.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReference-Eigenschaft. Gibt den Typ dieser Referenz zurück"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Ermittelt den Typ dieser Referenz.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;

            // Fügen Sie dem VBA-Projekt eine registrierte Referenz hinzu
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Rufen Sie die erste Referenz ab und demonstrieren Sie die Type-Eigenschaft
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Speichere die Arbeitsmappe
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Siehe auch

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


