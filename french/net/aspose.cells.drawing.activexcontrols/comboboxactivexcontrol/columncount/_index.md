---
title: "ComboBoxActiveXControl.ColumnCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Représente le nombre de colonnes à afficher dans une ComboBox ou une ListBox"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/
---
## ComboBoxActiveXControl.ColumnCount property

Représente le nombre de colonnes à afficher dans un ComboBox ou ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnCountDemo
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

            // Ajouter le contrôle ActiveX ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété ColumnCount et d'autres propriétés
            comboBox.ColumnCount = 1;
            comboBox.ListWidth = 100;
            comboBox.Value = "Apple;Banana;Cherry";

            // Enregistrez le classeur
            workbook.Save("ComboBoxColumnCountDemo.xlsx");

            Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
        }
    }
}
```

### Voir aussi

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


