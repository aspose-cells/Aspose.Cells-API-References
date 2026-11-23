---
title: "RevisionRenameSheet.NewName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionRenameSheet. Obtient le nouveau nom de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

Obtient le nouveau nom de la feuille de calcul.

```csharp
public string NewName { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyNewNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et la renommer pour déclencher une révision
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

            // Enregistrer dans un flux mémoire pour générer des révisions
            System.IO.MemoryStream ms = new System.IO.MemoryStream();
            workbook.Save(ms, SaveFormat.Xlsx);

            // Rouvrir le classeur pour accéder aux journaux de révisions
            workbook = new Workbook(ms);
            
            // Vérifier les journaux de révisions pour l'opération de renommage
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // Démontrer l'utilisation de la propriété NewName
                        if (renameSheet.NewName == newName)
                        {
                            Console.WriteLine("NewName property verification successful");
                        }
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


