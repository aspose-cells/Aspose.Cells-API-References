---
title: "ActiveXControlBase.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Indique si ce contrôle est visible"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

Indique si ce contrôle est visible.

```csharp
public virtual bool IsVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // Configurer les propriétés de base
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // Enregistrez le classeur
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


