---
title: "RevisionQueryTable.FieldId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionQueryTable. Obtient l'ID du champ de tableau de requête spécifique qui a été supprimé"
type: docs
url: /fr/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Obtient l'ID du champ de tableau de requête spécifique qui a été supprimé.

```csharp
public int FieldId { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Créer un tableau de requête (c'est un exemple simplifié)
                // Remarque : dans un scénario réel, vous devez d'abord créer un tableau de requête
                // À des fins de démonstration, nous allons simuler l'accès à un RevisionQueryTable

                // Comme nous ne pouvons pas créer directement un RevisionQueryTable dans cet exemple simplifié,
                // nous allons démontrer comment accéder à la propriété FieldId si nous en avions une
                // Cela montre le modèle pour lire la propriété en lecture seule

                // Simuler l'obtention d'un RevisionQueryTable à partir des révisions (conceptuel)
                // En réalité, vous obtiendriez cela à partir de workbook.Revisions ou similaire
                RevisionQueryTable revisionQueryTable = null;

                // Vérifiez si nous avons un tableau de requête de révision (c'est juste pour la démonstration)
                if (revisionQueryTable != null)
                {
                    // Afficher la valeur de la propriété FieldId
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Afficher d'autres propriétés pour le contexte
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Enregistrez le classeur
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


