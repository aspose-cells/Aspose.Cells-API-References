---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReference-egenskap. Hämtar och anger det utökade Libid för referensen"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Hämtar och anger det utökade Libid för referensen.

```csharp
public string ExtendedLibid { get; set; }
```

### Anmärkningar

Endast för kontrollreferens.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Initiera VBA-projekt
                VbaProject vbaProject = workbook.VbaProject;

                // Lägg till en kontrollreferens för att demonstrera ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Hämta den första referensen
                VbaProjectReference reference = vbaProject.References[0];

                // Visa värdet för ExtendedLibid-egenskapen
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Demonstrera att sätta ExtendedLibid (eftersom den är läs/skriv)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Spara arbetsboken
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

### Se även

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


