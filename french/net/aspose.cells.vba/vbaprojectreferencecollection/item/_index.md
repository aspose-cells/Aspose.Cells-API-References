---
title: "VbaProjectReferenceCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProjectReferenceCollection. Obtenez la référence dans la liste par l'index"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Obtenez la référence dans la liste par l'index.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Paramètre | Description |
| --- | --- |
| i | L'indice. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter des références au projet VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Obtenir la collection de références
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Accéder aux références en utilisant la propriété Item
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Enregistrez le classeur
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


