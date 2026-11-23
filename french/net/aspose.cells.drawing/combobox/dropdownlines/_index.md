---
title: "ComboBox.DropDownLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBox. Obtient ou définit le nombre de lignes de liste affichées dans la partie déroulante d'une boîte combinée"
type: docs
url: /fr/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Obtient ou définit le nombre de lignes de liste affichées dans la partie déroulante d'une boîte combinée.

```csharp
public int DropDownLines { get; set; }
```

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une ComboBox avec les paramètres corrects
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Remplir les cellules de la feuille de calcul avec des éléments
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Lier la boîte combinée aux valeurs des cellules
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


