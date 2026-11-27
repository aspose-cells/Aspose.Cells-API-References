---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReferenceCollection-metoden. Lägg till en referens till ett twiddlat typbibliotek och dess utökade typbibliotek"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Lägg till en referens till ett vridet typbibliotek och dess utökade typbibliotek.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på referensen. |
| libid | String | Identifieraren för ett Automation-typbibliotek. |
| twiddledlibid | String | Identifieraren för ett twiddlat typbibliotek |
| extendedLibid | String | Identifieraren för ett utökat typbibliotek |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället VbaProjectReferenceCollection.AddControlReferernce() metoden. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Lägg till kontrollreferens med alla strängparametrar
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


