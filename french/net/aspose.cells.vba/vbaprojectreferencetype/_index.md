---
title: "Énumération VbaProjectReferenceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Vba.VbaProjectReferenceType. Représente le type de référence de projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Représente le type de référence du projet VBA.

```csharp
public enum VbaProjectReferenceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Registered | `0` | Spécifie une référence à une bibliothèque de types Automation. |
| Control | `1` | Spécifie une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue. |
| Project | `2` | Spécifie une référence à un projet VBA externe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Ajouter une référence de projet VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Enregistrement du fichier Excel
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Démonstration de l'utilisation de l'énumération VbaProjectReferenceType
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


