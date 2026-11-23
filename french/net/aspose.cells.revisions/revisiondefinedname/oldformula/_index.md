---
title: "RevisionDefinedName.OldFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionDefinedName. Obtient l'ancienne formule"
type: docs
url: /fr/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Obtient l'ancienne formule.

```csharp
public string OldFormula { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez un nom défini pour générer l'historique des révisions
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifier le nom défini pour créer une révision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Enregistrez le classeur pour conserver les révisions
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Rouvrir le classeur pour accéder aux journaux de révisions
                Workbook revisionWorkbook = new Workbook(filePath);

                // Itérez à travers les journaux de révision pour trouver les révisions de noms définis
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
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

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


