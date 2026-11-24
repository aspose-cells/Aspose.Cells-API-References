---
title: "VbaProject.References"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Ruft alle Verweise des VBA-Projekts ab."
type: docs
url: /de/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Liest alle Verweise des VBA-Projekts.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe (VBA-Projekt wird für .xlsm-Dateien automatisch erstellt).
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf die VBA-Projektverweise zu (nur verfügbar, wenn die Arbeitsmappe ein VBA-Projekt enthält).
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Fügen Sie verschiedene Arten von Verweisen hinzu.
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Referenzanzahl anzeigen
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Als makrofähige Arbeitsmappe speichern
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


