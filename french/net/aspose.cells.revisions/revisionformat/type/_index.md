---
title: "RevisionFormat.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionFormat. Obtient le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Obtient le type de révision.

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

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur en mode partagé pour activer le suivi des révisions
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données et appliquez un formatage pour créer une révision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Appliquez un style pour créer une révision de format
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Accédez aux journaux de révision
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Afficher la valeur de la propriété Type
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Afficher des informations supplémentaires sur la révision
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


