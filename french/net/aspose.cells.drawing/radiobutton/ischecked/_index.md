---
title: "RadioButton.IsChecked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RadioButton. Indique si le bouton radio est coché ou non"
type: docs
url: /fr/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Indique si le bouton radio est coché ou non.

```csharp
public bool IsChecked { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un bouton radio à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Définir le texte du bouton radio
            radioButton.Text = "Option 1";
            
            // Initialement décoché
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Cocher le bouton radio
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Enregistrez le classeur
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


