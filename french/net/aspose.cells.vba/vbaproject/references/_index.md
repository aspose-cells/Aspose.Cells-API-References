---
title: "VbaProject.References"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Obtient toutes les références du projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Récupère toutes les références du projet VBA.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Créer un classeur (le projet VBA est créé automatiquement pour les fichiers .xlsm)
            Workbook workbook = new Workbook();
            
            // Accéder aux références du projet VBA (disponible uniquement si le classeur possède un projet VBA)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Ajouter différents types de références
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Afficher le nombre de références
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Enregistrer en tant que classeur avec macros
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Voir aussi

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


