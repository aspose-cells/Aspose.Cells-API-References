---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReference-Eigenschaft. Ruft den erweiterten Libid der Referenz ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Ermittelt und setzt die erweiterte Libid der Referenz.

```csharp
public string ExtendedLibid { get; set; }
```

### Hinweise

Nur für Steuerungsreferenz.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // VBA-Projekt initialisieren
                VbaProject vbaProject = workbook.VbaProject;

                // Fügen Sie eine Steuerungsreferenz hinzu, um ExtendedLibid zu demonstrieren
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Rufen Sie die erste Referenz ab
                VbaProjectReference reference = vbaProject.References[0];

                // Zeigen Sie den Wert der ExtendedLibid-Eigenschaft an
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Demonstrieren Sie das Setzen von ExtendedLibid (da es les- und schreibbar ist)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Speichere die Arbeitsmappe
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


