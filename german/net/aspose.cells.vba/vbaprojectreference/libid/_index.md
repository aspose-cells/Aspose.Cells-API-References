---
title: "VbaProjectReference.Libid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReference-Eigenschaft. Liest und schreibt die Libid der Referenz"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Ermittelt und setzt die Libid der Referenz.

```csharp
public string Libid { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook targetWorkbook = new Workbook();
            
            // Lade die Quellarbeitsmappe mit VBA-Projekt
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Lösche vorhandene Referenzen im Ziel
            targetWorkbook.VbaProject.References.Clear();
            
            // Kopiere Referenzen von der Quelle zum Ziel
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Demonstriere die Verwendung der Libid-Eigenschaft
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Ergebnis speichern
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


