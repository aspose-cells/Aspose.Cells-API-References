---
title: VbaModule
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le module dans le projet VBA.
type: docs
weight: 6240
url: /fr/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Représente le module dans le projet VBA.

```csharp
public class VbaModule
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Codes](../../aspose.cells.vba/vbamodule/codes) { get; set; } | Obtient et définit les codes du module. |
| [Name](../../aspose.cells.vba/vbamodule/name) { get; set; } | Obtient et définit le nom du module. |
| [Type](../../aspose.cells.vba/vbamodule/type) { get; } | Obtient le type de module. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
 // Initier le projet VBA.
VbaProject vbaProject = workbook.VbaProject; 
// Ajoute un nouveau module.
int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
// Récupère le module vba
VbaModule vbaModule = vbaProject.Modules[index];
// Définir les codes
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
//Enregistrement du fichier Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Lancer le projet VBA.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Ajouter un nouveau module.
Dim index as Integer = vbaProject.Modules.Add(VbaModuleType.Class, "test")
'Obtenir le module vba
Dim vbaModule as VbaModule = vbaProject.Modules(index)
'Définir des codes
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
'Enregistrement du fichier Excel
workbook.Save("book1.xlsm")
```

### Voir également

* espace de noms [Aspose.Cells.Vba](../../aspose.cells.vba)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
