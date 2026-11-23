---
title: "RadioButtonActiveXControl.IsWordWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RadioButtonActiveXControl. Indique si le contenu du contrôle se renvoie automatiquement à la fin d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/iswordwrapped/
---
## RadioButtonActiveXControl.IsWordWrapped property

Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX RadioButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton = 
                (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;

            // Démontrer la propriété IsWordWrapped
            Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = true;
            Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = false;
            Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);

            // Enregistrez le classeur
            workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


