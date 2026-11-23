---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Obtient et définit la couleur OLE de l'arrière-plan"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Obtient et définit la couleur ole de l'arrière-plan.

```csharp
public int BorderOleColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ComboBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de base
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Démontrer la propriété BorderOleColor
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Définir un texte d'exemple
            comboBox.Value = "Border Color Demo";

            // Enregistrez le classeur
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


