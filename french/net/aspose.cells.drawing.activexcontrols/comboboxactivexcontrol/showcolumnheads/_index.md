---
title: "ComboBoxActiveXControl.ShowColumnHeads"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Indique si les en-têtes de colonne sont affichés"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/
---
## ComboBoxActiveXControl.ShowColumnHeads property

Indique si les en-têtes de colonne sont affichés.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ComboBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Définissez les propriétés de la ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListWidth = 100;
            
            // Ajouter des données d'exemple au ComboBox
            comboBox.ListFillRange = "A1:B3";
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Value1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Value2");

            // Démontrer la propriété ShowColumnHeads
            Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
            
            // Activer les en-têtes de colonne
            comboBox.ShowColumnHeads = true;
            Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
            
            // Désactiver les en-têtes de colonne
            comboBox.ShowColumnHeads = false;
            Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);

            // Enregistrez le classeur
            workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


