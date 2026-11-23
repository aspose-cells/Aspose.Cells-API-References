---
title: "Classe UnknownControl"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.UnknownControl classe. Contrôle inconnu"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Contrôle inconnu.

```csharp
public class UnknownControl : ActiveXControl
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtient et définit la couleur ole de l'arrière-plan. (Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Obtient et définit les données binaires du contrôle. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Représente la police du contrôle. (Hérité de [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtient et définit la couleur ole du premier plan. (Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtient et définit la hauteur du contrôle en points. (Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Obtient et définit le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus. (Hérité de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. (Hérité de [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. (Hérité de [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indique si les données du contrôle sont verrouillées pour l'édition. (Hérité de [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indique si le contrôle est transparent.(Hérité de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indique si ce contrôle est visible.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtient et définit la cellule liée.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtient et définit la plage de remplissage de la liste.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtient et définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtient et définit le type d'icône affiché comme pointeur de la souris pour le contrôle.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indique s'il faut afficher une ombre.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Représente la façon d'aligner le texte utilisé par le contrôle.(Hérité de [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | Obtient le type du contrôle ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtient et définit la largeur du contrôle en points.(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtient l'objet [`Workbook`](../activexcontrolbase/workbook/).(Hérité de [`ActiveXControlBase`](../activexcontrolbase/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | Obtient les données associées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle Unknown ActiveX à la feuille de calcul
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Obtenez l'instance UnknownControl à partir de la forme
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Enregistrez le classeur
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


