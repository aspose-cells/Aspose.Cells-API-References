---
title: "Workbook.RemoveMacro"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Supprime le VBA/macro de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Supprime le VBA/macro de cette feuille de calcul.

```csharp
public void RemoveMacro()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir d'un fichier contenant des macros
            Workbook workbook = new Workbook("example.xlsm");

            // Supprimer les macros du classeur
            workbook.RemoveMacro();
            
            // Enregistrer comme classeur sans macro
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


