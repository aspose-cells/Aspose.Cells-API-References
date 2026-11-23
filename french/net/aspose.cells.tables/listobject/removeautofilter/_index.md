---
title: "ListObject.RemoveAutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Supprime le filtre automatique appliqué à ce tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/removeautofilter/
---
## ListObject.RemoveAutoFilter method

Supprime le filtre automatique appliqué à ce tableau.

```csharp
public void RemoveAutoFilter()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Remplir les données d'exemple (avec ligne d'en-tête)
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("Alice");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Bob");
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B4"].PutValue("Charlie");

            try
            {
                // Ajouter un ListObject (tableau) qui inclut un filtre automatique par défaut
                int listIndex = sheet.ListObjects.Add("A1", "B4", true);
                ListObject listObj = sheet.ListObjects[listIndex];

                // Optionnel : appliquer un filtre pour démontrer qu'un filtre existe
                listObj.Filter();

                // Supprimer le filtre automatique du ListObject
                listObj.RemoveAutoFilter();

                Console.WriteLine("RemoveAutoFilter called successfully.");
                
                // Enregistrer le classeur pour vérifier les modifications
                workbook.Save("RemoveAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during RemoveAutoFilter operation: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


