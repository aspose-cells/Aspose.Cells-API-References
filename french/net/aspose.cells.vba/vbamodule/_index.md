---
title: "Classe VbaModule"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Vba.VbaModule classe. Représente le module dans le projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Représente le module dans le projet VBA.

```csharp
public class VbaModule
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Obtient et définit les codes binaires du module. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Obtient et définit les codes du module. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Obtient et définit le nom du module. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Obtient le type du module. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Ajouter un nouveau module
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Obtenir le module VBA
            VbaModule vbaModule = vbaProject.Modules[index];

            // Définir les codes pour le module
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Enregistrement du fichier Excel
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


