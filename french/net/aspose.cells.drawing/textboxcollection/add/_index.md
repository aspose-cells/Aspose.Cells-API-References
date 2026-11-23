---
title: "TextBoxCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextBoxCollection. Ajoute une zone de texte à la collection"
type: docs
url: /fr/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Ajoute un textbox à la collection.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| hauteur | Int32 | Hauteur de la zone de texte, en unité de pixel. |
| largeur | Int32 | Largeur de la zone de texte, en unité de pixel. |

### Valeur de retour

[`TextBox`](../../textbox/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### Voir aussi

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


