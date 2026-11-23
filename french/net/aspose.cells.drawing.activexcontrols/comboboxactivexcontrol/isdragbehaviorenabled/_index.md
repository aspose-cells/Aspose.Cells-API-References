---
title: "ComboBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Indique si le glisser‑déposer est activé pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/
---
## ComboBoxActiveXControl.IsDragBehaviorEnabled property

Indique si le glisser-déposer est activé pour le contrôle.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ComboBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Définir quelques propriétés de base
            comboBox.ListRows = 8;
            comboBox.ColumnCount = 1;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = -1;

            // Démontrer la propriété IsDragBehaviorEnabled
            Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
            
            // Désactiver le comportement de glissement
            comboBox.IsDragBehaviorEnabled = false;
            Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
            
            // Activer le comportement de glissement
            comboBox.IsDragBehaviorEnabled = true;
            Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);

            // Enregistrez le classeur
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


