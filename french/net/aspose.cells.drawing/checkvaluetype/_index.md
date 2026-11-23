---
title: "Énumération CheckValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.CheckValueType. Représente le type de valeur de case à cocher"
type: docs
url: /fr/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Représente le type de valeur de coche de la case à cocher.

```csharp
public enum CheckValueType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| UnChecked | `0` | Non coché |
| Checked | `1` | Coché |
| Mixed | `2` | Mixte |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des cases à cocher à la feuille de calcul
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Obtenez les cases à cocher et définissez leurs propriétés
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Définir les valeurs des cases à cocher et l'état coché
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Lier les cases à cocher aux cellules
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Afficher les valeurs des cellules pour démontrer le lien
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


