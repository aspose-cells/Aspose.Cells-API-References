---
title: "ListBoxActiveXControl.BorderStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBoxActiveXControl. Obtient et définit le type de bordure utilisé par le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderstyle/
---
## ListBoxActiveXControl.BorderStyle property

Obtient et définit le type de bordure utilisé par le contrôle.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter le contrôle ListBox ActiveX avec des paramètres corrigés
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                1, 0, 1, 100, 150, 30); // Added height parameter
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété BorderStyle
            listBox.BorderStyle = ControlBorderType.None;

            // Vérifier et afficher le style de bordure
            Console.WriteLine("BorderStyle: " + listBox.BorderStyle);

            workbook.Save("ListBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


