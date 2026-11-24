---
title: "Aufzählung VbaProjectReferenceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaProjectReferenceType-Enum. Stellt den Typ einer VBA-Projektreferenz dar"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Stellt den Typ der VBA‑Projekt‑Referenz dar.

```csharp
public enum VbaProjectReferenceType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Registered | `0` | Gibt eine Referenz auf eine Automation-Typbibliothek an. |
| Control | `1` | Gibt eine Referenz auf eine manipulierte Typbibliothek und deren erweiterte Typbibliothek an. |
| Project | `2` | Gibt eine Referenz auf ein externes VBA-Projekt an. |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;

            // VBA-Projektreferenz hinzufügen
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Die Excel-Datei speichern
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Demonstration der Verwendung des VbaProjectReferenceType-Enums
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


