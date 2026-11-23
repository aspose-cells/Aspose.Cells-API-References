---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ComboBoxActiveXControl property. Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus.

```csharp
public bool HideSelection { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ComboBox ActiveX avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de base
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Ajouter des éléments d'exemple en utilisant le nom de propriété correct
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Démontrer la propriété HideSelection
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Enregistrez le classeur
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


