---
title: "SpinButtonActiveXControl.Max"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpinButtonActiveXControl. Obtient et définit la valeur maximale acceptable"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Obtient et définit la valeur maximale acceptable.

```csharp
public int Max { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un contrôle ActiveX SpinButton à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Obtenez le contrôle ActiveX et définissez sa propriété Max
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Enregistrez le classeur
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


