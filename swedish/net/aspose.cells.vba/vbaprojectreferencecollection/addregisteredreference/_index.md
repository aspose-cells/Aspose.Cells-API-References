---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReferenceCollection-metoden. Lägg till en referens till ett Automation-typbibliotek"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Lägg till en referens till ett automations-typbibliotek.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på referensen. |
| libid | String | Identifieraren för ett Automation-typbibliotek. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en registrerad referens till stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Spara arbetsboken
            workbook.Save("output.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


