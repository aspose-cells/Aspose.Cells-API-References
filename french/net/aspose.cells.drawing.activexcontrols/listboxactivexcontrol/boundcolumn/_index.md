---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ListBoxActiveXControl propriété. Représente comment la propriété Value est déterminée pour un ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est fmMultiSelectSingle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

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
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Ajouter le contrôle ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de ListBox
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // Définir BoundColumn à 0 (colonne ID) - ce sera la valeur renvoyée lorsqu'un élément est sélectionné
            listBox.BoundColumn = 0;
            
            // Définir TextColumn à 1 (colonne Nom) - cela sera affiché dans la liste
            listBox.TextColumn = 1;

            // Enregistrez le classeur
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Voir aussi

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


