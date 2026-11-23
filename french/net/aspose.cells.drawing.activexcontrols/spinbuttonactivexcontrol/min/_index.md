---
title: "SpinButtonActiveXControl.Min"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpinButtonActiveXControl. Obtient et définit la valeur minimale acceptable"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Obtient et définit la valeur minimale acceptable.

```csharp
public int Min { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un contrôle ActiveX SpinButton à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Définir la propriété Min du SpinButton
            spinButton.Min = 0;
            
            // Définir d'autres propriétés pour démontrer la fonctionnalité
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Enregistrez le classeur
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


