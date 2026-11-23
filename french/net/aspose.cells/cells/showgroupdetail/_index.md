---
title: "Cells.ShowGroupDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Développe les lignes/colonnes groupées"
type: docs
url: /fr/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Développe les lignes/colonnes groupées.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isVertical | Boolean | Vrai, développe les lignes groupées. |
| indice | Int32 | L'index de ligne/colonne |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données d'exemple dans les lignes 5-7 (index basé sur zéro : 4-6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Grouper les lignes 4-6 (lignes Excel 5-7) et les réduire initialement
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Développer les lignes groupées en utilisant ShowGroupDetail (isVertical : false pour les lignes, index : 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


