---
title: "Enumération SelectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enumération Aspose.Cells.Drawing.SelectionType. Le type de sélection de la zone de liste"
type: docs
url: /fr/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Le type de sélection de la zone de liste.

```csharp
public enum SelectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Single | `0` | Type de sélection unique. |
| Multi | `1` | Type de sélection multiple. |
| Extend | `2` | Étendre le type de sélection. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de liste à la feuille de calcul
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Définir le type de sélection sur Simple
            listBox.SelectionType = SelectionType.Single;

            // Ajouter des éléments à la zone de liste
            listBox.SetInputRange("A1:A5", false, false);

            // Vérifier le type de sélection
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Enregistrez le classeur
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


