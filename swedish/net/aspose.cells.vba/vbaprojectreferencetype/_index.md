---
title: "Enum VbaProjectReferenceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaProjectReferenceType enum. Representerar typen av VBA-projektreferens"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Representerar typen av VBA‑projektreferens.

```csharp
public enum VbaProjectReferenceType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Registered | `0` | Anger en referens till ett Automation-typbibliotek. |
| Control | `1` | Anger en referens till ett justerat typbibliotek och dess utökade typbibliotek. |
| Project | `2` | Anger en referens till ett externt VBA-projekt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Lägg till VBA-projektreferens
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Sparar Excel-filen
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Demonstrerar användningen av VbaProjectReferenceType enum
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


