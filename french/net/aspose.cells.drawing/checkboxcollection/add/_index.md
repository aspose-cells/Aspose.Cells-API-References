---
title: "CheckBoxCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CheckBoxCollection. Ajoute une case à cocher à la collection"
type: docs
url: /fr/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Ajoute un checkBox à la collection.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| hauteur | Int32 | Hauteur de la case à cocher, en pixels. |
| largeur | Int32 | Largeur de la case à cocher, en pixels. |

### Valeur de retour

[`CheckBox`](../../checkbox/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une case à cocher en utilisant les paramètres Int32 (upperLeftRow, upperLeftColumn, height, width)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


