---
title: "TextBoxCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextBoxCollection. Supprime une zone de texte du fichier"
type: docs
url: /fr/net/aspose.cells.drawing/textboxcollection/removeat/
---
## TextBoxCollection.RemoveAt method

Supprime une zone de texte du fichier.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de la zone de texte. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez quelques zones de texte à la feuille de calcul
            for (int i = 0; i < 3; i++)
            {
                worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
                worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
            }

            Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);

            // Supprimez la dernière zone de texte en utilisant RemoveAt avec le paramètre Int32
            int lastIndex = worksheet.TextBoxes.Count - 1;
            worksheet.TextBoxes.RemoveAt(lastIndex);

            Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
        }
    }
}
```

### Voir aussi

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


