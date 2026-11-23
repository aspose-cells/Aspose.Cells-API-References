---
title: "CheckBoxActiveXControl.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Indique si le contrôle est coché ou non"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Indique si le contrôle est coché ou non.

```csharp
public CheckValueType Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX CheckBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Définissez les propriétés de base incluant Value
            checkBox.Caption = "Check Me";
            checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage

            // Enregistrez le classeur
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


