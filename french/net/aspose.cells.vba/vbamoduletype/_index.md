---
title: "Énumération VbaModuleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Vba.VbaModuleType. Représente le type de module VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Représente le type de module VBA.

```csharp
public enum VbaModuleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Procedural | `0` | Représente un module procédural. |
| Document | `1` | Représente un module de document. |
| Class | `2` | Représente un module de classe. |
| Designer | `3` | Représente un module de concepteur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter un nouveau module de classe
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Obtenir le module VBA
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Définir les codes pour le module
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Enregistrez le fichier Excel
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


