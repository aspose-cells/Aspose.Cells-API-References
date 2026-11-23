---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Indique si les objets liés aux dessins tels que les images, formes, graphiques... seront considérés comme vides. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Remarques

Lorsque cette propriété est définie sur false, toutes les lignes/colonnes couvertes par des objets de dessin ne seront pas considérées comme vides et ne seront pas supprimées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Ajoutez un objet de dessin pour tester le comportement de DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Supprimer les colonnes vides avec DrawingsAsBlank = false (préserve les dessins)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Voir aussi

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


