---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProjectReference. Obtient et définit le Libid étendu de la référence"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Obtient et définit le Libid étendu de la référence.

```csharp
public string ExtendedLibid { get; set; }
```

### Remarques

Uniquement pour la référence de contrôle.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Initialiser le projet VBA
                VbaProject vbaProject = workbook.VbaProject;

                // Ajouter une référence de contrôle pour démontrer ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Obtenir la première référence
                VbaProjectReference reference = vbaProject.References[0];

                // Afficher la valeur de la propriété ExtendedLibid
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Démontrer la définition de ExtendedLibid (puisqu'il est en lecture/écriture)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Enregistrez le classeur
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


