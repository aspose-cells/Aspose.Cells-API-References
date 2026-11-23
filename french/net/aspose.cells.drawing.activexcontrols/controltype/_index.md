---
title: "Enum ControlType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Représente tous les types de contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controltype/
---
## ControlType enumeration

Représente tous les types de contrôle ActiveX.

```csharp
public enum ControlType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| CommandButton | `0` | Bouton |
| ComboBox | `1` | Boîte combinée |
| CheckBox | `2` | Case à cocher |
| ListBox | `3` | Boîte de liste |
| TextBox | `4` | Zone de texte |
| SpinButton | `5` | Sélecteur |
| RadioButton | `6` | Bouton radio |
| Label | `7` | Étiquette |
| Image | `8` | Image |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | Barre de défilement |
| BarCode | `11` | Barre de défilement |
| Unknown | `12` | Inconnu |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlTypeDemo
    {
        public static void ControlTypeExample()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX CommandButton
            Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
            ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
            commandButtonControl.IsEnabled = true;
            commandButtonControl.IsVisible = true;

            // Ajouter un contrôle ActiveX ComboBox
            Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
            ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
            comboBoxControl.IsEnabled = true;
            comboBoxControl.IsVisible = true;

            // Ajouter un contrôle ActiveX CheckBox
            Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
            ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
            checkBoxControl.IsEnabled = true;
            checkBoxControl.IsVisible = true;

            // Ajouter un contrôle ActiveX ListBox
            Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
            ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
            listBoxControl.IsEnabled = true;
            listBoxControl.IsVisible = true;

            // Ajouter un contrôle ActiveX TextBox
            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
            ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsVisible = true;

            // Ajouter un contrôle ActiveX SpinButton
            Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
            ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
            spinButtonControl.IsEnabled = true;
            spinButtonControl.IsVisible = true;

            // Ajouter un contrôle ActiveX RadioButton
            Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
            ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
            radioButtonControl.IsEnabled = true;
            radioButtonControl.IsVisible = true;

            // Ajouter un contrôle ActiveX Label
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
            ActiveXControl labelControl = labelShape.ActiveXControl;
            labelControl.IsEnabled = true;
            labelControl.IsVisible = true;

            // Ajouter un contrôle ActiveX Image
            Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
            ActiveXControl imageControl = imageShape.ActiveXControl;
            imageControl.IsEnabled = true;
            imageControl.IsVisible = true;

            // Ajouter un contrôle ActiveX ToggleButton
            Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
            ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
            toggleButtonControl.IsEnabled = true;
            toggleButtonControl.IsVisible = true;

            // Ajouter un contrôle ActiveX ScrollBar
            Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
            ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
            scrollBarControl.IsEnabled = true;
            scrollBarControl.IsVisible = true;
                       

            // Enregistrez le classeur
            workbook.Save("ControlTypeExample.xlsx");
            workbook.Save("ControlTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


