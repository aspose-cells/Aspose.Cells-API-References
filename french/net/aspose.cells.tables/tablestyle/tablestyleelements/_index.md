---
title: "TableStyle.TableStyleElements"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyle. Récupère tous les éléments du style de tableau"
type: docs
url: /fr/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Obtient tous les éléments du style de tableau.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un tableau
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Obtenir le style de tableau (utiliser le style existant au lieu d'en créer un nouveau)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Modifier les éléments du style de tableau
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Appliquer le style modifié au tableau
            table.TableStyleName = style.Name;

            // Enregistrez le classeur
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


