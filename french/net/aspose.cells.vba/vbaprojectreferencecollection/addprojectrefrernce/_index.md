---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProjectReferenceCollection. Ajoute une référence à un projet VBA externe"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Ajoute une référence à un projet VBA externe.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la référence. |
| absoluteLibid | String | L'identifiant du projet VBA référencé avec un chemin absolu. |
| relativeLibid | String | L'identifiant du projet VBA référencé avec un chemin relatif. |

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode VbaProjectReferenceCollection.AddProjectReferernce(). Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter une référence de projet avec des libids absolus et relatifs
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Afficher le nombre de références
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Enregistrez le classeur
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


