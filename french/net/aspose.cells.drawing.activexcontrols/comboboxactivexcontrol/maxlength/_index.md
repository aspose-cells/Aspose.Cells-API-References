---
title: "ComboBoxActiveXControl.MaxLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ComboBoxActiveXControl property. Obtient et définit le nombre maximal de caractères"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/
---
## ComboBoxActiveXControl.MaxLength property

Obtient et définit le nombre maximal de caractères

```csharp
public int MaxLength { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ComboBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété MaxLength et les autres propriétés essentielles
            comboBox.MaxLength = 10; // Restrict input to 10 characters
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;
            comboBox.Value = "Test";

            // Enregistrez le classeur
            workbook.Save("ComboBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


