---
title: "ListBox.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBox. Indique si la combobox a un ombrage 3D"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

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
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les éléments de la liste
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Créer la listbox et définir les propriétés principales
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Définir la propriété shadow
            listBox.Shadow = true;

            // Enregistrez et rechargez pour vérifier
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Voir aussi

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


