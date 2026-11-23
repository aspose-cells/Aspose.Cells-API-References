---
title: "Enum ShowDropButtonType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Spécifie quand afficher le bouton déroulant"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Spécifie quand afficher le bouton déroulant

```csharp
public enum ShowDropButtonType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Never | `0` | Ne jamais afficher le bouton déroulant. |
| Focus | `1` | Afficher le bouton déroulant lorsque le contrôle a le focus. |
| Always | `2` | Toujours afficher le bouton déroulant. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ComboBox à la feuille de calcul
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Définir les propriétés du contrôle ActiveX ComboBox
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Ajouter quelques éléments à la ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Enregistrez le classeur
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


