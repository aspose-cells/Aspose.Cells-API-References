---
title: "ComboBoxActiveXControl.BoundColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ComboBoxActiveXControl property. Représente la façon dont la propriété Value est déterminée pour un ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est fmMultiSelectSingle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/
---
## ComboBoxActiveXControl.BoundColumn property

Représente la façon dont la propriété Value est déterminée pour un ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est (fmMultiSelectSingle).

```csharp
public int BoundColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Ajouter un contrôle ActiveX ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurer le ComboBox
            comboBox.ListFillRange = "A1:B4";
            comboBox.ColumnCount = 2;
            comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
            comboBox.TextColumn = 1; // Display the Name column (column index 1)

            // Enregistrez le classeur
            workbook.Save("ComboBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


