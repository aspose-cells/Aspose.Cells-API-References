---
title: "CheckBoxActiveXControl.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Obtient le type du contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

Obtient le type du contrôle ActiveX.

```csharp
public override ControlType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX CheckBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Définir les propriétés
            checkBox.Caption = "Sample CheckBox";
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;
            checkBox.IsEnabled = true;

            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
            if (checkBox.Type == ControlType.CheckBox)
            {
                Console.WriteLine("This is a CheckBox control");
            }

            // Enregistrez le classeur
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


