---
title: "ListColumn.GetDataStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListColumn. Obtient le style des données dans cette colonne du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

Obtient le style des données dans cette colonne du tableau.

```csharp
public Style GetDataStyle()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Créer un objet liste (table)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Obtenez le style du premier ListColumn
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Modifier le style
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Appliquez à nouveau le style modifié à la colonne
            table.ListColumns[0].SetDataStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


