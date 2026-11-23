---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProjectReferenceCollection. Ajouter une référence à une bibliothèque de types Automation"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Ajoutez une référence à une bibliothèque de types Automation.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la référence. |
| libid | String | L'identifiant d'une bibliothèque de types Automation. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder au projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter une référence enregistrée à stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


