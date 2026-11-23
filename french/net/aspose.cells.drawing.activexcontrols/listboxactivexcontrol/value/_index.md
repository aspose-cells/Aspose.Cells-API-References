---
title: "ListBoxActiveXControl.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBoxActiveXControl. Obtient et définit la valeur du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Obtient et définit la valeur du contrôle.

```csharp
public string Value { get; set; }
```

### Remarques

S'applique uniquement lorsque [`SelectionType`](../selectiontype/) est SelectionType.Single;

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Définir les propriétés de base
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Définir les éléments en utilisant la propriété Value
            listBox.Value = "Red;Green;Blue;Yellow";

            // Enregistrez le classeur
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Voir aussi

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


