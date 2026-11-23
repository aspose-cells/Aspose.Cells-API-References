---
title: "Classe ActiveXControlBase"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControlBase classe. Représente le contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/
---
## ActiveXControlBase class

Représente le contrôle ActiveX.

```csharp
public abstract class ActiveXControlBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtient et définit la couleur ole de l'arrière-plan. |
| virtual [Data](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/data/) { get; } | Obtient et définit les données binaires du contrôle. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtient et définit la couleur OLE du premier plan. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtient et définit la hauteur du contrôle en unité de points. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indique si ce contrôle est visible. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtient et définit la cellule liée. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtient et définit la plage de remplissage de la liste. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtient et définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtient et définit le type d'icône affichée comme pointeur de la souris pour le contrôle. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indique s'il faut afficher une ombre. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Obtient le type du contrôle ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtient et définit la largeur du contrôle en unité de points. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtient l'objet [`Workbook`](./workbook/). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBaseDemo
    {
        public static void ActiveXControlBaseExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Définir les propriétés du contrôle ActiveX
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = "A1";
            control.ListFillRange = "A2:A10";

            // Enregistrez le classeur
            workbook.Save("ActiveXControlBaseExample.xlsx");
            workbook.Save("ActiveXControlBaseExample.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


