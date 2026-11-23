---
title: "VbaProjectReference.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProjectReference. Obtient et définit le nom de la référence"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Obtient et définit le nom de la référence.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un classeur (le projet VBA est créé automatiquement pour les fichiers .xlsm)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Ajouter une référence au projet VBA
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Accéder et vérifier la référence par la propriété Name
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Enregistrez le classeur
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


