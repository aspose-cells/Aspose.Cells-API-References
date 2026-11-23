---
title: "CheckBox.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBox. Indique si la case à cocher possède un ombrage 3D"
type: docs
url: /fr/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Indique si la zone de liste déroulante possède un ombrage 3D.

```csharp
public bool Shadow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une case à cocher à la feuille de calcul et obtenir son indice
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Configurer les propriétés de la case à cocher
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Démontrer la propriété Shadow
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


