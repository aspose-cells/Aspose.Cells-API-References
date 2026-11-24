---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReferenceCollection-Methode. Fügt eine Referenz zu einem externen VBA-Projekt hinzu"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Fügt einen Verweis zu einem externen VBA-Projekt hinzu.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Referenz. |
| absoluteLibid | String | Der Bezeichner des referenzierten VBA-Projekts mit einem absoluten Pfad. |
| relativeLibid | String | Der Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad. |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode VbaProjectReferenceCollection.AddProjectReferernce(). Diese Methode wird 12 Monate nach Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;
            
            // Fügen Sie eine Projektreferenz mit absoluten und relativen LibIDs hinzu
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Referenzanzahl anzeigen
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Speichere die Arbeitsmappe
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


