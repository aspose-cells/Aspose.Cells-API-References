---
title: "ActiveXControlBase.ListFillRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Obtient et définit la plage de remplissage de la liste"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

Obtient et définit la plage de remplissage de la liste.

```csharp
public string ListFillRange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour ListFillRange
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // Ajouter un ComboBoxActiveXControl
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Définir ListFillRange pour remplir la combobox
            comboBox.ListFillRange = "A2:A10";

            // Enregistrez le classeur
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


