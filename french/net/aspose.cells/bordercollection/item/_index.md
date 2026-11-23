---
title: "BorderCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BorderCollection. Obtient l’élément Border à l’index spécifié"
type: docs
url: /fr/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Obtient l’élément [`Border`](../../border/) à l’index spécifié.

```csharp
public Border this[BorderType borderType] { get; }
```

| Paramètre | Description |
| --- | --- |
| borderType | La bordure à récupérer. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Obtenir la cellule et son style
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Accéder à la BorderCollection depuis le style
                BorderCollection borders = style.Borders;

                // Afficher la valeur actuelle de la propriété Item (opération de lecture)
                // Remarque : la propriété Item est en lecture seule et renvoie un objet Border
                // La propriété Item nécessite un paramètre BorderType
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Enregistrer le résultat
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


