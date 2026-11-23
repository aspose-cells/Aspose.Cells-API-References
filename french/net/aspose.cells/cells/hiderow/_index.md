---
title: "Cells.HideRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Masque une ligne"
type: docs
url: /fr/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Masque une ligne.

```csharp
public void HideRow(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Masquer la ligne 5
            worksheet.Cells.HideRow(5);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


