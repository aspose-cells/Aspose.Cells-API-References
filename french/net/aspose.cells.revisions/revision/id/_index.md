---
title: "Revision.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Revision. Obtient le numéro de cette révision"
type: docs
url: /fr/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Obtient le numéro de cette révision.

```csharp
public int Id { get; }
```

### Remarques

Zero signifie que cette révision ne contient pas d'ID.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Effectuez une modification pour potentiellement créer une révision
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Obtenez la collection des journaux de révision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Obtenez les révisions du premier journal
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Accédez à la première révision
                        Revision revision = revisions[0];
                        
                        // Affichez la propriété Id (lecture seule)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Enregistrez le classeur
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
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

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


