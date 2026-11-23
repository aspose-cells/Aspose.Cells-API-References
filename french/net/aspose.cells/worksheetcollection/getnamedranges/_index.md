---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Récupère toutes les plages nommées prédéfinies dans le classeur"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Obtient toutes les plages nommées pré‑définies dans la feuille de calcul.

```csharp
public Range[] GetNamedRanges()
```

### Valeur de retour

Un tableau d'objets Range. Si la référence du nom défini est externe ou possède plusieurs plages, aucun objet Range ne sera retourné pour ce nom.

Renvoie null si la plage nommée n'existe pas.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer quelques plages nommées à des fins de démonstration
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Appeler la méthode GetNamedRanges pour récupérer toutes les plages nommées
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Afficher les informations sur les plages nommées
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Enregistrez le classeur
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


