---
title: "RadioButton.GetOptionIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RadioButton. Obtient l'index d'option basé sur 1 dans tous les boutons radio du GroupBox qui contient ce bouton radio"
type: docs
url: /fr/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

Obtient l'index de l'option (à partir de 1) parmi tous les boutons radio du GroupBox qui contient ce bouton radio.

```csharp
public int GetOptionIndex()
```

### Remarques

Si ce bouton radio n'est pas dans le GroupBox, renvoie l'index d'option parmi tous les boutons radio qui ne sont dans aucun GroupBox

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un group box pour contenir les boutons radio
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // Ajouter trois boutons radio au GroupBox
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // Définir les boutons radio comme faisant partie du GroupBox
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // Obtenir l'index d'option pour chaque bouton radio
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // Cocher le premier bouton radio pour démontrer la sélection
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


