---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReferenceCollection-Methode. Fügt eine Referenz zu einer Automation-Typbibliothek hinzu"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Füge einen Verweis zu einer Automation-Typbibliothek hinzu.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Referenz. |
| libid | String | Der Bezeichner einer Automation-Typbibliothek. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Registrierte Referenz zu stdole hinzufügen
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


