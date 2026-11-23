---
title: "RevisionQueryTable.CellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionQueryTable. Obtient l'emplacement du tableau de requête affecté"
type: docs
url: /fr/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Obtient l'emplacement du tableau de requête affecté.

```csharp
public CellArea CellArea { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
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
                RevisionQueryTable revisionQueryTable = null;

                // Vérifiez si nous avons un tableau de requête de révision
                if (revisionQueryTable != null)
                {
                    // Afficher la valeur de la propriété CellArea (lecture seule)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Afficher d'autres propriétés pour le contexte
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Enregistrez le classeur
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


