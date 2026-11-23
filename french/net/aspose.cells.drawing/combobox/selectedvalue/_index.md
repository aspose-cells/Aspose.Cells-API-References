---
title: "ComboBox.SelectedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBox. Obtient la valeur sélectionnée de la boîte combinée"
type: docs
url: /fr/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Obtient la valeur sélectionnée de la boîte combinée.

```csharp
public string SelectedValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un ComboBox et ajouter des éléments
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Définir les valeurs dans la plage d'entrée
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // Démontrer SelectedValue (propriété en lecture seule)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Enregistrez le classeur
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


