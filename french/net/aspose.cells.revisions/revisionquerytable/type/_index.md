---
title: "RevisionQueryTable.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionQueryTable. Représente le type de la révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Représente le type de la révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyTypeDemo
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
                // Dans un scénario réel, vous obtiendriez les révisions à partir du workbook
                // Pour la démonstration, nous créerons un exemple conceptuel
                // Remarque : les instances de RevisionQueryTable sont généralement obtenues à partir des révisions du classeur

                // Créer un RevisionQueryTable factice (c'est conceptuel - en réalité vous l'obtiendriez à partir des révisions)
                // Comme nous ne pouvons pas instancier directement RevisionQueryTable, nous démontrerons le modèle
                RevisionQueryTable revisionQueryTable = null;

                // Vérifiez si nous avons un tableau de requête de révision
                if (revisionQueryTable != null)
                {
                    // Afficher la valeur de la propriété Type (lecture seule)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Afficher la valeur de l'énumération en tant qu'entier pour référence
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Afficher d'autres propriétés pour le contexte
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Enregistrez le classeur
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


