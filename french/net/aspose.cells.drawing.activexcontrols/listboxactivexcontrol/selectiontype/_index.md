---
title: "ListBoxActiveXControl.SelectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ListBoxActiveXControl propriété. Indique si le contrôle autorise plusieurs sélections"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Indique si le contrôle autorise plusieurs sélections.

```csharp
public SelectionType SelectionType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Ajouter le contrôle ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            
            // Démontrer la propriété SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.Value = "Apple;Banana;Cherry";

            // Enregistrez le classeur
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");

            Console.WriteLine("ListBox with Single SelectionType created successfully.");
        }
    }
}
```

### Voir aussi

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


