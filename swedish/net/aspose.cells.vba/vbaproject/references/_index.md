---
title: "VbaProject.References"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Hämtar alla referenser för VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Hämtar alla referenser för VBA-projektet.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Exempel

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
            // Skapa en arbetsbok (VBA-projekt skapas automatiskt för .xlsm-filer)
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektets referenser (endast tillgängligt om arbetsboken har VBA-projekt)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Lägg till olika typer av referenser
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Visa referensantalet
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Spara som makroaktiverad arbetsbok
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


