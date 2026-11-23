---
title: "Classe RevisionDefinedName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionDefinedName. Représente un enregistrement de révision d'un changement de nom défini"
type: docs
url: /fr/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Représente un enregistrement de révision d'une modification de nom défini.

```csharp
public class RevisionDefinedName : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Obtient la formule. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Obtient l'ancienne formule. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Obtient le texte du nom défini. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Représente le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter un nom défini au classeur
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifier le nom défini pour créer une révision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Enregistrer le classeur pour générer les journaux de révision
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Rouvrir le classeur pour accéder aux informations de révision
                Workbook revisionWorkbook = new Workbook(filePath);

                // Itérer à travers les journaux de révision pour trouver les entrées RevisionDefinedName
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Afficher les propriétés de RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
                        }
                    }
                }
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


