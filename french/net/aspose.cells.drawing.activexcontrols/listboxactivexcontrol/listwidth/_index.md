---
title: "ListBoxActiveXControl.ListWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ListBoxActiveXControl propriété. Obtient et définit la largeur en unités de points"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/listwidth/
---
## ListBoxActiveXControl.ListWidth property

Obtient et définit la largeur en points.

```csharp
public double ListWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ListBox ActiveX avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                10, 10, 200, 100, 200, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété ListWidth
            listBox.ListWidth = 150;
            
            // Configurer les propriétés de base
            listBox.ColumnCount = 2;
            listBox.ColumnWidths = 100; // Changed from string to double
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Red");
            worksheet.Cells["B2"].PutValue("Yellow");
            worksheet.Cells["B3"].PutValue("Orange");
            
            // Définir la plage de données
            listBox.ListFillRange = "A1:B3";

            workbook.Save("ListBoxWidthDemo.xlsx");
            Console.WriteLine("ListBox with ListWidth=150 created successfully.");
        }
    }
}
```

### Voir aussi

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


