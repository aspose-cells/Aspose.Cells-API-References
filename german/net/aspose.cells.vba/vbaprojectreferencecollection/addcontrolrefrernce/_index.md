---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReferenceCollection-Methode. Eine Referenz zu einer gedrehten Typbibliothek und ihrer erweiterten Typbibliothek hinzufügen"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Füge einen Verweis zu einer manipulierten Typbibliothek und ihrer erweiterten Typbibliothek hinzu.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Referenz. |
| libid | String | Der Bezeichner einer Automation-Typbibliothek. |
| twiddledlibid | String | Der Bezeichner einer gedrehten Typbibliothek |
| extendedLibid | String | Der Bezeichner einer erweiterten Typbibliothek |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode VbaProjectReferenceCollection.AddControlReferernce(). Diese Methode wird 12 Monate nach Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

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

            // Steuerungsreferenz mit allen String-Parametern hinzufügen
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

### Siehe auch

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


