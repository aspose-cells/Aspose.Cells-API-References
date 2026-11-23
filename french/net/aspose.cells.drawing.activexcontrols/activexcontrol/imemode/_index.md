---
title: "ActiveXControl.IMEMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControl. Obtient et définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Obtient et définit le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ToggleButton avec les coordonnées appropriées
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Définir les propriétés incluant IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Vérifier et afficher la propriété IMEMode
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Enregistrez le classeur
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


