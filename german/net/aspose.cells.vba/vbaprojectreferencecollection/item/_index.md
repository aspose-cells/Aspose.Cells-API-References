---
title: "VbaProjectReferenceCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReferenceCollection-Eigenschaft. Gibt die Referenz in der Liste anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Erhalte den Verweis in der Liste nach dem Index.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| i | Der Index. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;
            
            // Referenzen zum VBA-Projekt hinzufügen
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Referenzsammlung abrufen
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Auf Referenzen über die Item-Eigenschaft zugreifen
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


