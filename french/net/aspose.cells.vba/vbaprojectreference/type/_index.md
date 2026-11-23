---
title: "VbaProjectReference.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProjectReference. Obtient le type de cette référence"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Obtient le type de cette référence.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Ajouter une référence enregistrée au projet VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Obtenir la première référence et démontrer la propriété Type
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Enregistrez le classeur
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Voir aussi

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


