---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProjectReferenceCollection. Ajoutez une référence à une bibliothèque de types twiddled et à sa bibliothèque de types étendue"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la référence. |
| libid | String | L'identifiant d'une bibliothèque de types Automation. |
| twiddledlibid | String | L'identifiant d'une bibliothèque de types twiddled |
| extendedLibid | String | L'identifiant d'une bibliothèque de types étendue |

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode VbaProjectReferenceCollection.AddControlReferernce(). Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Ajouter une référence de contrôle avec tous les paramètres de chaîne
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


