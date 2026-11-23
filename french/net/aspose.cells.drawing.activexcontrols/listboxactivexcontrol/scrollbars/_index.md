---
title: "ListBoxActiveXControl.ScrollBars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBoxActiveXControl. Indique si le contrôle possède des barres de défilement verticales, horizontales, les deux ou aucune"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBoxControl = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Ajouter quelques éléments pour rendre les barres de défilement visibles
            listBoxControl.ListFillRange = "A1:A20";
            for (int i = 1; i <= 20; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }

            // Démontrer la propriété ScrollBars
            listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;

            workbook.Save("ListBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


