---
title: "ListObject.UpdateColumnName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Met à jour le nom de toutes les colonnes de la liste vers les cellules du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Met à jour le nom de toutes les colonnes de liste dans les cellules du tableau.

```csharp
public void UpdateColumnName()
```

### Remarques

La valeur des cellules de la ligne d'en-tête du tableau doit être identique au nom du ListColumn ; Cell.PutValue ne modifie pas automatiquement le nom du ListColumn pour des raisons de performance.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Créer un objet tableau/liste
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Peupler le tableau avec quelques données
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Mettre à jour les noms de colonnes (définira des noms par défaut comme Column1, Column2, etc.)
            listObject.UpdateColumnName();

            // Enregistrez le classeur
            wb.Save("output.xlsx");

            // Vérifier que le nom de la colonne a été mis à jour
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


