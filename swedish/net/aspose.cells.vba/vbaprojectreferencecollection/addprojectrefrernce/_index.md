---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReferenceCollection metod. Lägger till en referens till ett externt VBA-projekt"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Lägger till en referens till ett externt VBA-projekt.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på referensen. |
| absoluteLibid | String | Den refererade VBA-projektets identifierare med en absolut sökväg. |
| relativeLibid | String | Den refererade VBA-projektets identifierare med en relativ sökväg |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället VbaProjectReferenceCollection.AddProjectReferernce() metoden. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en projektreferens med absoluta och relativa libid
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Visa referensantalet
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Spara arbetsboken
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


