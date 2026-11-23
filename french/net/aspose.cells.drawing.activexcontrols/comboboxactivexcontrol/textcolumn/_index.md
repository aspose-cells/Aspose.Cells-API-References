---
title: "ComboBoxActiveXControl.TextColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Représente la colonne dans une ComboBox ou une ListBox à afficher à l'utilisateur"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/
---
## ComboBoxActiveXControl.TextColumn property

Représente la colonne d'une ComboBox ou d'une ListBox à afficher à l'utilisateur.

```csharp
public int TextColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyTextColumnDemo
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

            // Configurer les propriétés de la ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 5;
            
            // Ajouter des éléments en utilisant ListFillRange (alternative à AddItem)
            worksheet.Cells["A1"].PutValue("Item1");
            worksheet.Cells["B1"].PutValue("Description1");
            worksheet.Cells["A2"].PutValue("Item2");
            worksheet.Cells["B2"].PutValue("Description2");
            worksheet.Cells["A3"].PutValue("Item3");
            worksheet.Cells["B3"].PutValue("Description3");
            comboBox.ListFillRange = "A1:B3";

            // Démontrer la propriété TextColumn
            comboBox.TextColumn = 2; // Display second column (descriptions) as text
            comboBox.BoundColumn = 1; // But bind to first column (items)

            // Enregistrez le classeur
            workbook.Save("ComboBoxTextColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


