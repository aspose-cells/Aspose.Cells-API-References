---
title: "Énumération ControlMousePointerType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType. Représente le type d'icône affichée comme pointeur de souris pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Représente le type d'icône affiché comme pointeur de souris pour le contrôle.

```csharp
public enum ControlMousePointerType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Pointeur standard. |
| Arrow | `1` | Flèche. |
| Cross | `2` | Pointeur croix. |
| IBeam | `3` | I-beam. |
| SizeNESW | `6` | Double flèche pointant au nord-est et au sud-ouest. |
| SizeNS | `7` | Double flèche pointant au nord et au sud. |
| SizeNWSE | `8` | Double flèche pointant au nord-ouest et au sud-est. |
| SizeWE | `9` | Double flèche pointant à l'ouest et à l'est. |
| UpArrow | `10` | Flèche vers le haut. |
| HourGlass | `11` | Sablier. |
| NoDrop | `12` | \"Not\" symbole (cercle avec une ligne diagonale) au-dessus de l'objet en cours de déplacement. |
| AppStarting | `13` | Flèche avec un sablier. |
| Help | `14` | Flèche avec un point d'interrogation. |
| SizeAll | `15` | \"Size-all\" curseur (flèches pointant au nord, au sud, à l'est et à l'ouest). |
| Custom | `99` | Utilise l'icône spécifiée par la propriété MouseIcon. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Effectuez un cast du ActiveXControl vers ActiveXControlBase pour accéder à ses propriétés
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Définissez le type de pointeur de la souris pour le contrôle
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Définissez d'autres propriétés à des fins de démonstration
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Enregistrez le classeur
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Afficher le résultat
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


