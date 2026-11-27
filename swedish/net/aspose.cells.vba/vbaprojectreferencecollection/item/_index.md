---
title: "VbaProjectReferenceCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReferenceCollection egenskap. Hämta referensen i listan efter indexet"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Hämta referensen i listan efter index.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| i | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till referenser till VBA-projektet
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Hämta referenssamling
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Åtkomst till referenser med Item-egenskapen
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Spara arbetsboken
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


