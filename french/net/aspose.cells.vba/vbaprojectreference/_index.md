---
title: "Classe VbaProjectReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Vba.VbaProjectReference. Représente la référence du projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Représente la référence du projet VBA.

```csharp
public class VbaProjectReference
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Obtient et définit le Libid étendu de la référence. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Obtient et définit le Libid de la référence. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Obtient et définit le nom de la référence. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Obtient et définit l'identifiant du projet VBA référencé avec un chemin relatif. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Obtient et définit le Libid modifié de la référence. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Obtient le type de cette référence. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
 // Initialiser le projet VBA.
VbaProject vbaProject = workbook.VbaProject;
// Ajouter une référence de projet VBA
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Enregistrement du fichier Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### Voir aussi

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


