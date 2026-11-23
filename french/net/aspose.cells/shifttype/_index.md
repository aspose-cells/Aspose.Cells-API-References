---
title: "Énumération ShiftType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.ShiftType. Représente les options de décalage lors de la suppression d'une plage de cellules"
type: docs
url: /fr/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Représente les options de décalage lors de la suppression d'une plage de cellules.

```csharp
public enum ShiftType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Down | `0` | Décaler les cellules vers le bas. |
| Left | `1` | Décaler les cellules vers la gauche. |
| None | `2` | Ne pas décaler les cellules. |
| Right | `3` | Décaler les cellules vers la droite. |
| Up | `4` | Décaler les cellules vers le haut. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Insérer une nouvelle ligne à l'index 1, en décalant les lignes existantes vers le bas
            worksheet.Cells.InsertRows(1, 1, true);

            // Définir une valeur dans la ligne nouvellement insérée
            worksheet.Cells["A1"].PutValue("New Item");

            // Supprimer une plage de cellules et décaler les cellules vers le haut
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Afficher les valeurs restantes dans la première colonne
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Enregistrez le classeur
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


