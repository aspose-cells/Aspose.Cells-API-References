---
title: "RevisionFormat.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionFormat. Obtient le style appliqué"
type: docs
url: /fr/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Obtient le style appliqué.

```csharp
public Style Style { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur (le suivi des révisions est activé par défaut lorsque des modifications sont apportées)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données et du formatage pour créer une révision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Créer un style et l'appliquer à la cellule
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Accéder aux révisions via RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Afficher les propriétés de style actuelles de la révision
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Remarque : la propriété Style est en lecture seule dans RevisionFormat, nous ne pouvons donc pas la modifier directement
                        // Pour modifier le formatage, nous devrions modifier directement le style de la cellule
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


