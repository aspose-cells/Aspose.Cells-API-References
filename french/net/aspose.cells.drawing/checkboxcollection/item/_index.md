---
title: "CheckBoxCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxCollection. Obtient l'élément CheckBox à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Obtient l'élément [`CheckBox`](../../checkbox/) à l'index spécifié.

```csharp
public CheckBox this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une case à cocher à la feuille de calcul
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Accédez à la case à cocher en utilisant la propriété Item (indexeur)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Accédez à la case à cocher en utilisant l'index (propriété Item)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Affichez les propriétés de la case à cocher
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Enregistrez le classeur
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


