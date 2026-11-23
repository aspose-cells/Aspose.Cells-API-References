---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Spécifie l'unité de base utilisée pour étendre une sélection. True indique que l'unité de base est un caractère unique. false indique que l'unité de base est un mot complet"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

Spécifie l'unité de base utilisée pour étendre une sélection. True indique que l'unité de base est un caractère unique. false indique que l'unité de base est un mot entier.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ComboBox ActiveX avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de base
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // Démontrer la propriété IsAutoWordSelected
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Enregistrez le classeur
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


