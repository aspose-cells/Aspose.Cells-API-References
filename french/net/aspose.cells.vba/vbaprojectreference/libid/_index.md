---
title: "VbaProjectReference.Libid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProjectReference. Obtient et définit le Libid de la référence"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Obtient et définit le Libid de la référence.

```csharp
public string Libid { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook targetWorkbook = new Workbook();
            
            // Charger le classeur source avec le projet VBA
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Effacer les références existantes dans la cible
            targetWorkbook.VbaProject.References.Clear();
            
            // Copier les références de la source vers la cible
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Démontrer l'utilisation de la propriété Libid
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Enregistrer le résultat
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


