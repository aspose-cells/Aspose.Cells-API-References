---
title: "Workbook.CopyTheme"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Copie le thème d'un autre classeur"
type: docs
url: /fr/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Copie le thème d'un autre classeur.

```csharp
public void CopyTheme(Workbook source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Classeur | Classeur source. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Créer un classeur source (le thème est automatiquement défini lors de l'ouverture d'un fichier modèle)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            
            // Copier le thème du classeur source vers le classeur de destination
            destWorkbook.CopyTheme(sourceWorkbook);

            // Enregistrer le classeur de destination
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


