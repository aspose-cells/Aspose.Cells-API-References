---
title: "Classe RevisionQueryTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionQueryTable. Représente une révision d'une modification de champ de tableau de requête"
type: docs
url: /fr/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Représente une révision d'une modification de champ de tableau de requête.

```csharp
public class RevisionQueryTable : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Obtient l'emplacement du tableau de requête affecté. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Obtient l'ID du champ de tableau de requête spécifique qui a été supprimé. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Représente le type de la révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajoutez des données d'exemple pour créer un contexte pour la table de requête
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Remarque : les instances de RevisionQueryTable sont généralement obtenues à partir des révisions du classeur
                // Il s'agit d'une démonstration conceptuelle car nous ne pouvons pas instancier directement RevisionQueryTable

                // Dans un scénario réel, vous accéderiez aux révisions comme ceci :
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Access properties
                //     }
                // }

                // À des fins de démonstration, nous montrerons comment travailler avec les propriétés de RevisionQueryTable
                // si nous avions une instance
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Enregistrez le classeur
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


