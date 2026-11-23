---
title: "Cells.HideGroupDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Réduit les lignes/colonnes groupées"
type: docs
url: /fr/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Réduit les lignes/colonnes groupées.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isVertical | Boolean | True, réduire les lignes groupées. |
| indice | Int32 | L'index de ligne/colonne |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Groupez les lignes et masquez les détails
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

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


