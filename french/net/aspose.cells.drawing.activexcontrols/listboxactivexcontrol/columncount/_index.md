---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ListBoxActiveXControl propriété. Représente le nombre de colonnes à afficher dans un ComboBox ou ListBox"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Représente le nombre de colonnes à afficher dans un ComboBox ou ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Définir les propriétés incluant ColumnCount
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // Vérifier et afficher le ColumnCount
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

            // Enregistrez le classeur
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


