---
title: "RevisionDefinedName.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionDefinedName. Obtient le texte du nom défini"
type: docs
url: /fr/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Obtient le texte du nom défini.

```csharp
public string Text { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez un nom défini
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Modifiez le nom défini pour générer une révision
            name.RefersTo = "=Sheet1!$B$1";
            
            // Enregistrez dans le fichier pour générer des révisions
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Rouvrez le fichier pour lire les révisions
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Vérifiez les révisions
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


