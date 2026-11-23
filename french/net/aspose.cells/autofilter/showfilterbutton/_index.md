---
title: "AutoFilter.ShowFilterButton"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFilter. Indique si le bouton AutoFilter pour cette colonne est visible"
type: docs
url: /fr/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Indique si le bouton AutoFilter pour cette colonne est visible.

```csharp
public bool ShowFilterButton { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un objet liste/tableau
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Activer l'autofiltre et afficher les boutons de filtre
            table.AutoFilter.ShowFilterButton = true;

            // Enregistrez le classeur
            workbook.Save("output_with_filter_buttons.xlsx");

            // Masquer les boutons de filtre
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


